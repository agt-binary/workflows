The following query gets all active clients who have had some kind of limit placed on them.

```postgresql
select distinct on (loginid) loginid, stamp, custom_max_daily_turnover, custom_max_payout, 
       pg_userid, place_of_birth, residence, citizen, aml_risk_classification
  from audit.client 
  where ((custom_max_daily_turnover > 0 or custom_max_payout > 0) and operation='UPDATE')
        and ((pg_userid <> 'write') and (pg_userid <> 'system'))
  order by loginid, stamp desc;
```
