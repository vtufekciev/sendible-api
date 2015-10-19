To retrieve daily statistics for a given social media account detail, make a GET call using basic authentication. The days returned represent the date for the given year/month period.

#### URL: ####
http://sendible.com/api/v1/account-statistics.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_detail_id`: The account detail id for which to retrieve the valid `yearmonth` codes. Valid `account_detail_id`s can be retrieved using the using the [GetAccountDetails](GetAccountDetails.md) call.
  * `yearmonth`: Optional. The `yearmonth` period for which to retrieve statistics. Valid `yearmonth`s can be retrieved using the using the [GetAccountPeriods](GetAccountPeriods.md) call.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<account-statistics type="array">
 <account-statistic>
  <code>Fans</code>
  <day-1 type="decimal">7575.0</day-1>
  <day-10 type="decimal">7653.0</day-10>
  <day-11 type="decimal">7663.0</day-11>
  <day-12 type="decimal">7674.0</day-12>
  <day-13 type="decimal">7692.0</day-13>
  <day-14 type="decimal">7704.0</day-14>
  <day-15 type="decimal">7719.0</day-15>
  <day-16 type="decimal">7730.0</day-16>
  <day-17 type="decimal">7743.0</day-17>
  <day-18 type="decimal">7751.0</day-18>
  <day-19 type="decimal">7761.0</day-19>
  <day-2 type="decimal">7568.0</day-2>
  <day-20 type="decimal">7773.0</day-20>
  <day-21 type="decimal">7786.0</day-21>
  <day-22 type="decimal">7795.0</day-22>
  <day-23 type="decimal">7804.0</day-23>
  <day-24 type="decimal">7813.0</day-24>
  <day-25 type="decimal">7827.0</day-25>
  <day-26 type="decimal">7843.0</day-26>
  <day-27 type="decimal">7861.0</day-27>
  <day-28 type="decimal">7873.0</day-28>
  <day-29 type="decimal">7889.0</day-29>
  <day-3 type="decimal">7587.0</day-3>
  <day-30 type="decimal">7901.0</day-30>
  <day-31 type="decimal">7913.0</day-31>
  <day-4 type="decimal">7594.0</day-4>
  <day-5 type="decimal">7610.0</day-5>
  <day-6 type="decimal">7619.0</day-6>
  <day-7 type="decimal">7627.0</day-7>
  <day-8 type="decimal">7635.0</day-8>
  <day-9 type="decimal">7645.0</day-9>
  <id type="integer">3975268</id>
  <yearmonth>201203</yearmonth>
</account-statistic>
<account-statistic>
  <code>Page Views</code>
  <day-1 type="decimal">207.0</day-1>
  <day-10 type="decimal">252.0</day-10>
  <day-11 type="decimal">201.0</day-11>
  <day-12 type="decimal">288.0</day-12>
  <day-13 type="decimal">188.0</day-13>
  <day-14 type="decimal">202.0</day-14>
  <day-15 type="decimal">186.0</day-15>
  <day-16 type="decimal">200.0</day-16>
  <day-17 type="decimal">221.0</day-17>
  <day-18 type="decimal">213.0</day-18>
  <day-19 type="decimal">226.0</day-19>
  <day-2 type="decimal">228.0</day-2>
  <day-20 type="decimal">173.0</day-20>
  <day-21 type="decimal">199.0</day-21>
  <day-22 type="decimal">177.0</day-22>
  <day-23 type="decimal">177.0</day-23>
  <day-24 type="decimal">213.0</day-24>
  <day-25 type="decimal">206.0</day-25>
  <day-26 type="decimal">232.0</day-26>
  <day-27 type="decimal">188.0</day-27>
  <day-28 type="decimal">193.0</day-28>
  <day-29 type="decimal">260.0</day-29>
  <day-3 type="decimal">181.0</day-3>
  <day-30 type="decimal">221.0</day-30>
  <day-31 type="decimal">248.0</day-31>
  <day-4 type="decimal">226.0</day-4>
  <day-5 type="decimal">210.0</day-5>
  <day-6 type="decimal">210.0</day-6>
  <day-7 type="decimal">153.0</day-7>
  <day-8 type="decimal">166.0</day-8>
  <day-9 type="decimal">249.0</day-9>
  <id type="integer">4137142</id>
 <yearmonth>201203</yearmonth>
</account-statistic>
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```