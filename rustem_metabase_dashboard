Client's name
```sql
SELECT CONCAT_WS(' ', salutation, first_name, last_name) AS name
FROM betonmarkets.client
where true [[and binary_user_id = {{binary_userid}}]]  [[and email like CONCAT({{email}}, '%')]] [[and loginid = {{Account_loginid}}]]
LIMIT 1
```
Client's country
```sql
select
    case
        when residence = 'ad' then 'Andorra'
        when residence = 'ae' then 'United Arab Emirates'
        when residence = 'af' then 'Afghanistan'
        when residence = 'ag' then 'Antigua and Barbuda'
        when residence = 'ai' then 'Anguilla'
        when residence = 'al' then 'Albania'
        when residence = 'am' then 'Armenia'
        when residence = 'ao' then 'Angola'
        when residence = 'aq' then 'Antarctica'
        when residence = 'ar' then 'Argentina'
        when residence = 'at' then 'Austria'
        when residence = 'au' then 'Australia'
        when residence = 'aw' then 'Aruba'
        when residence = 'ax' then 'Aland Islands'
        when residence = 'az' then 'Azerbaijan'
        when residence = 'ba' then 'Bosnia and Herzegovina'
        when residence = 'bb' then 'Barbados'
        when residence = 'bd' then 'Bangladesh'
        when residence = 'be' then 'Belgium'
        when residence = 'bf' then 'Burkina Faso'
        when residence = 'bg' then 'Bulgaria'
        when residence = 'bh' then 'Bahrain'
        when residence = 'bi' then 'Burundi'
        when residence = 'bj' then 'Benin'
        when residence = 'bl' then 'Saint Barthelemy'
        when residence = 'bm' then 'Bermuda'
        when residence = 'bn' then 'Brunei Darussalam'
        when residence = 'bo' then 'Bolivia (Plurinational State of)'
        when residence = 'br' then 'Brazil'
        when residence = 'bs' then 'Bahamas'
        when residence = 'bt' then 'Bhutan'
        when residence = 'bv' then 'Bouvet Island'
        when residence = 'bw' then 'Botswana'
        when residence = 'by' then 'Belarus'
        when residence = 'bz' then 'Belize'
        when residence = 'cc' then 'Cocos (Keeling) Islands'
        when residence = 'cd' then 'Congo (The Democratic Republic of the)'
        when residence = 'cf' then 'Central African Republic'
        when residence = 'cg' then 'Congo'
        when residence = 'ch' then 'Switzerland'
        when residence = 'ci' then 'Cote d''Ivoire'
        when residence = 'ck' then 'Cook Islands'
        when residence = 'cl' then 'Chile'
        when residence = 'cm' then 'Cameroon'
        when residence = 'cn' then 'China'
        when residence = 'co' then 'Colombia'
        when residence = 'cu' then 'Cuba'
        when residence = 'cv' then 'Cabo Verde'
        when residence = 'cx' then 'Christmas Island'
        when residence = 'cy' then 'Cyprus'
        when residence = 'cz' then 'Czechia'
        when residence = 'de' then 'Germany'
        when residence = 'dj' then 'Djibouti'
        when residence = 'dk' then 'Denmark'
        when residence = 'dm' then 'Dominica'
        when residence = 'do' then 'Dominican Republic'
        when residence = 'dz' then 'Algeria'
        when residence = 'ec' then 'Ecuador'
        when residence = 'ee' then 'Estonia'
        when residence = 'eg' then 'Egypt'
        when residence = 'eh' then 'Western Sahara'
        when residence = 'er' then 'Eritrea'
        when residence = 'es' then 'Spain'
        when residence = 'et' then 'Ethiopia'
        when residence = 'fi' then 'Finland'
        when residence = 'fj' then 'Fiji'
        when residence = 'fk' then 'Falkland Islands (The) [Malvinas]'
        when residence = 'fm' then 'Micronesia (Federated States of)'
        when residence = 'fo' then 'Faroe Islands'
        when residence = 'fr' then 'France'
        when residence = 'ga' then 'Gabon'
        when residence = 'gb' then 'United Kingdom of Great Britain and Northern Ireland'
        when residence = 'gd' then 'Grenada'
        when residence = 'ge' then 'Georgia'
        when residence = 'gf' then 'French Guiana'
        when residence = 'gh' then 'Ghana'
        when residence = 'gi' then 'Gibraltar'
        when residence = 'gl' then 'Greenland'
        when residence = 'gm' then 'Gambia'
        when residence = 'gn' then 'Guinea'
        when residence = 'gp' then 'Guadeloupe'
        when residence = 'gq' then 'Equatorial Guinea'
        when residence = 'gr' then 'Greece'
        when residence = 'gs' then 'South Georgia and the South Sandwich Islands'
        when residence = 'gt' then 'Guatemala'
        when residence = 'gw' then 'Guinea-Bissau'
        when residence = 'gy' then 'Guyana'
        when residence = 'hm' then 'Heard Island and McDonald Islands'
        when residence = 'hn' then 'Honduras'
        when residence = 'hr' then 'Croatia'
        when residence = 'ht' then 'Haiti'
        when residence = 'hu' then 'Hungary'
        when residence = 'id' then 'Indonesia'
        when residence = 'ie' then 'Ireland'
        when residence = 'im' then 'Isle of Man'
        when residence = 'in' then 'India'
        when residence = 'io' then 'British Indian Ocean Territory'
        when residence = 'iq' then 'Iraq'
        when residence = 'is' then 'Iceland'
        when residence = 'it' then 'Italy'
        when residence = 'jm' then 'Jamaica'
        when residence = 'jo' then 'Jordan'
        when residence = 'ke' then 'Kenya'
        when residence = 'kg' then 'Kyrgyzstan'
        when residence = 'kh' then 'Cambodia'
        when residence = 'ki' then 'Kiribati'
        when residence = 'km' then 'Comoros'
        when residence = 'kn' then 'Saint Kitts and Nevis'
        when residence = 'kr' then 'Korea, The Republic of'
        when residence = 'kw' then 'Kuwait'
        when residence = 'ky' then 'Cayman Islands'
        when residence = 'kz' then 'Kazakhstan'
        when residence = 'la' then 'Lao People''s Democratic Republic'
        when residence = 'lb' then 'Lebanon'
        when residence = 'lc' then 'Saint Lucia'
        when residence = 'li' then 'Liechtenstein'
        when residence = 'lk' then 'Sri Lanka'
        when residence = 'lr' then 'Liberia'
        when residence = 'ls' then 'Lesotho'
        when residence = 'lt' then 'Lithuania'
        when residence = 'lu' then 'Luxembourg'
        when residence = 'lv' then 'Latvia'
        when residence = 'ly' then 'Libya'
        when residence = 'ma' then 'Morocco'
        when residence = 'mc' then 'Monaco'
        when residence = 'md' then 'Moldova, The Republic of'
        when residence = 'me' then 'Montenegro'
        when residence = 'mf' then 'Saint Martin (French part)'
        when residence = 'mg' then 'Madagascar'
        when residence = 'mh' then 'Marshall Islands'
        when residence = 'mk' then 'Macedonia, The former Yugoslav Republic of'
        when residence = 'ml' then 'Mali'
        when residence = 'mm' then 'Myanmar'
        when residence = 'mn' then 'Mongolia'
        when residence = 'mo' then 'Macao'
        when residence = 'mq' then 'Martinique'
        when residence = 'mr' then 'Mauritania'
        when residence = 'ms' then 'Montserrat'
        when residence = 'mu' then 'Mauritius'
        when residence = 'mv' then 'Maldives'
        when residence = 'mw' then 'Malawi'
        when residence = 'mx' then 'Mexico'
        when residence = 'mz' then 'Mozambique'
        when residence = 'na' then 'Namibia'
        when residence = 'nc' then 'New Caledonia'
        when residence = 'ne' then 'Niger'
        when residence = 'nf' then 'Norfolk Island'
        when residence = 'ng' then 'Nigeria'
        when residence = 'ni' then 'Nicaragua'
        when residence = 'nl' then 'Netherlands'
        when residence = 'no' then 'Norway'
        when residence = 'np' then 'Nepal'
        when residence = 'nr' then 'Nauru'
        when residence = 'nu' then 'Niue'
        when residence = 'nz' then 'New Zealand'
        when residence = 'om' then 'Oman'
        when residence = 'pa' then 'Panama'
        when residence = 'pe' then 'Peru'
        when residence = 'pf' then 'French Polynesia'
        when residence = 'pg' then 'Papua New Guinea'
        when residence = 'ph' then 'Philippines'
        when residence = 'pk' then 'Pakistan'
        when residence = 'pl' then 'Poland'
        when residence = 'pm' then 'Saint Pierre and Miquelon'
        when residence = 'pn' then 'Pitcairn'
        when residence = 'ps' then 'Palestine, State of'
        when residence = 'pt' then 'Portugal'
        when residence = 'pw' then 'Palau'
        when residence = 'py' then 'Paraguay'
        when residence = 'qa' then 'Qatar'
        when residence = 're' then 'Reunion'
        when residence = 'ro' then 'Romania'
        when residence = 'rs' then 'Serbia'
        when residence = 'ru' then 'Russian Federation'
        when residence = 'rw' then 'Rwanda'
        when residence = 'sa' then 'Saudi Arabia'
        when residence = 'sb' then 'Solomon Islands'
        when residence = 'sc' then 'Seychelles'
        when residence = 'sd' then 'Sudan'
        when residence = 'se' then 'Sweden'
        when residence = 'sg' then 'Singapore'
        when residence = 'sh' then 'Saint Helena, Ascension and Tristan da Cunha'
        when residence = 'si' then 'Slovenia'
        when residence = 'sj' then 'Svalbard and Jan Mayen'
        when residence = 'sk' then 'Slovakia'
        when residence = 'sl' then 'Sierra Leone'
        when residence = 'sm' then 'San Marino'
        when residence = 'sn' then 'Senegal'
        when residence = 'so' then 'Somalia'
        when residence = 'sr' then 'Suriname'
        when residence = 'st' then 'Sao Tome and Principe'
        when residence = 'sv' then 'El Salvador'
        when residence = 'sy' then 'Syrian Arab Republic'
        when residence = 'sz' then 'Swaziland'
        when residence = 'tc' then 'Turks and Caicos Islands'
        when residence = 'td' then 'Chad'
        when residence = 'tf' then 'French Southern Territories'
        when residence = 'tg' then 'Togo'
        when residence = 'th' then 'Thailand'
        when residence = 'tj' then 'Tajikistan'
        when residence = 'tk' then 'Tokelau'
        when residence = 'tl' then 'Timor-Leste'
        when residence = 'tm' then 'Turkmenistan'
        when residence = 'tn' then 'Tunisia'
        when residence = 'to' then 'Tonga'
        when residence = 'tr' then 'Turkey'
        when residence = 'tt' then 'Trinidad and Tobago'
        when residence = 'tv' then 'Tuvalu'
        when residence = 'tw' then 'Taiwan (Province of China)'
        when residence = 'tz' then 'Tanzania, United Republic of'
        when residence = 'ua' then 'Ukraine'
        when residence = 'ug' then 'Uganda'
        when residence = 'uy' then 'Uruguay'
        when residence = 'uz' then 'Uzbekistan'
        when residence = 'va' then 'Holy See'
        when residence = 'vc' then 'Saint Vincent and the Grenadines'
        when residence = 've' then 'Venezuela (Bolivarian Republic of)'
        when residence = 'vg' then 'Virgin Islands (British)'
        when residence = 'vn' then 'Viet Nam'
        when residence = 'wf' then 'Wallis and Futuna'
        when residence = 'ws' then 'Samoa'
        when residence = 'ye' then 'Yemen'
        when residence = 'yt' then 'Mayotte'
        when residence = 'za' then 'South Africa'
        when residence = 'zm' then 'Zambia'
        when residence = 'zw' then 'Zimbabwe'
        else 'Country code not found'
    end as country_of_residence
from betonmarkets.client
where true [[and binary_user_id = {{binary_userid}}]]  [[and email like CONCAT({{email}}, '%')]] [[and loginid = {{Account_loginid}}]]
limit 1
```

Client's account opening reason
```sql
SELECT account_opening_reason
FROM betonmarkets.client
where true [[and binary_user_id = {{binary_userid}}]]  [[and email like CONCAT({{email}}, '%')]] [[and loginid = {{Account_loginid}}]]
LIMIT 1
```
Client's join date.
```sql
SELECT date_joined
FROM betonmarkets.client
where true [[and binary_user_id = {{binary_userid}}]]  [[and email like CONCAT({{email}}, '%')]] [[and loginid = {{Account_loginid}}]]
ORDER BY date_joined ASC
LIMIT 1
```
Whether the client is connected to an affiliate.
```sql
select case
    when myaffiliates_token != '' then 'Affiliated'
    else 'Non-affiliated'
end
from betonmarkets.client
where true [[and binary_user_id = {{binary_userid}}]]  [[and email like CONCAT({{email}}, '%')]] [[and loginid = {{Account_loginid}}]]
limit 1
```

CLient's currency balances (if the client has multiple currency accounts).
```sql
SELECT loginid,
    currency_code,
    balance AS current_balance,
    last_modified
FROM (
  SELECT loginid
  FROM betonmarkets.client
  where true [[and binary_user_id = {{binary_userid}}]]  [[and email like CONCAT({{email}}, '%')]] [[and loginid = {{Account_loginid}}]]
) AS logins
LEFT JOIN transaction.account a on a.client_loginid = logins.loginid
ORDER BY loginid
```

Client's currency preference (if the client has multiple currency accounts)
```sql
SELECT currency_code, COUNT(*) AS contracts
FROM (
  SELECT id, a.currency_code
  FROM (
    SELECT loginid
    FROM betonmarkets.client
    where true [[and binary_user_id = {{binary_userid}}]]  [[and email like CONCAT({{email}}, '%')]] [[and loginid = {{Account_loginid}}]]
  ) AS logins
  LEFT JOIN transaction.account a ON a.client_loginid = logins.loginid
) AS account_ids
INNER JOIN transaction.transaction t ON t.account_id = account_ids.id
WHERE t.action_type='buy'
[[AND t.transaction_time >= {{purchase_since}}]]
GROUP BY 1
```

Client's market preference.
```sql
SELECT market, SUM(contracts) AS contracts
FROM (
    SELECT underlying_symbol, COUNT(*) AS contracts
    FROM (
      SELECT id
      FROM (
        SELECT loginid
        FROM betonmarkets.client
        where true [[and binary_user_id = {{binary_userid}}]]  [[and email like CONCAT({{email}}, '%')]] [[and loginid = {{Account_loginid}}]]
      ) AS logins
      LEFT JOIN transaction.account a ON a.client_loginid = logins.loginid
    ) AS account_ids
    INNER JOIN bet.financial_market_bet b ON b.account_id = account_ids.id
    [[WHERE b.purchase_time >= {{purchase_since}}]]
    GROUP BY underlying_symbol
) AS count_per_symbol
LEFT JOIN bet.market m ON m.symbol = count_per_symbol.underlying_symbol
GROUP BY 1
```

Client's app preference.
```sql
SELECT source, COUNT(*) AS contracts
FROM (
  SELECT id
  FROM (
    SELECT loginid
    FROM betonmarkets.client
    where true [[and binary_user_id = {{binary_userid}}]]  [[and email like CONCAT({{email}}, '%')]] [[and loginid = {{Account_loginid}}]]
  ) AS logins
  LEFT JOIN transaction.account a ON a.client_loginid = logins.loginid
) AS account_ids
INNER JOIN transaction.transaction t ON t.account_id = account_ids.id
WHERE t.action_type='buy'
[[AND t.transaction_time >= {{purchase_since}}]]
GROUP BY 1
```

Client's bet type preference.
```sql
SELECT bet_type, COUNT(*) AS contracts
FROM (
  SELECT id
  FROM (
    SELECT loginid
    FROM betonmarkets.client
    WHERE email in ({{email}})
  ) AS logins
  LEFT JOIN transaction.account a ON a.client_loginid = logins.loginid
) AS account_ids
INNER JOIN bet.financial_market_bet b ON b.account_id = account_ids.id
[[WHERE b.purchase_time >= {{purchase_since}}]]
GROUP BY 1
```

