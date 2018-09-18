The following query gets all the contracts purchased in a given date range.
```

with params as (select
       '2018-09-01'::TIMESTAMP AS start_date,
       '2018-12-31'::TIMESTAMP AS end_date
)
       
select output.*
from params
CROSS JOIN betonmarkets.production_servers_v2() as ps
CROSS JOIN dblink(ps.srvname,
$$
     select b.id, 
            b.purchase_time, 
            b.underlying_symbol, 
            b.payout_price, 
            b.buy_price, 
            b.sell_price, 
            b.start_time,
            b.expiry_time, 
            b.bet_type, 
            b.remark, 
            b.short_code, 
            b.sell_time, 
            a.client_loginid, 
            bm.market, 
            bm.submarket, 
            data_collection.exchangetousd_rate(a.currency_code, b.purchase_time) as "exchange_rate",
            c.residence,
            c.date_joined,
            b.tick_count,
            c.myaffiliates_token,
            t.source
     from only bet.financial_market_bet as b
     join transaction.transaction t on b.id=t.financial_market_bet_id and t.action_type='buy' --and t.source=6070
     join transaction.account a on a.id=b.account_id
     join betonmarkets.client c on c.loginid=a.client_loginid
     left join bet.market bm on b.underlying_symbol = bm.symbol
     where 
     --market <> 'volidx' and 
     --tick_count < 31 and
     --residence = 'in' and
     --client_loginid='CR684130' and
     
     --where market = 'forex' and
      --sell_time is not null and
     ((purchase_time between $$ || quote_literal(params.start_date) || $$::TIMESTAMP and $$ || quote_literal(params.end_date) || $$::TIMESTAMP) --or
           --(sell_time between $$ || quote_literal(params.start_date) || $$::TIMESTAMP and $$ || quote_literal(params.end_date) || $$::TIMESTAMP)
           )
      order by purchase_time
      limit 1000000 offset 0
$$) as output(id NUMERIC, 
        purchase_time TIMESTAMP, 
        underlying_symbol VARCHAR, 
        payout_price NUMERIC, 
        buy_price NUMERIC, 
        sell_price NUMERIC, 
        start_time TIMESTAMP, 
        expiry_time TIMESTAMP, 
        bet_type VARCHAR,
        remark VARCHAR, 
        short_code VARCHAR, 
        sell_time TIMESTAMP, 
        client_loginid VARCHAR,
        market VARCHAR,
        submarket VARCHAR,
        exchange_rate NUMERIC,
        residence VARCHAR,
        date_joined TIMESTAMP,
        tick_count NUMERIC,
        myaffiliates_token VARCHAR,
        source VARCHAR)
--where output.market in ('forex')
--order by output.purchase_time
--limit 1000000 offset 0

```
