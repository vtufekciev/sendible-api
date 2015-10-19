To retrieve a list of the valid periods for a given social media account detail, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/account-periods.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_detail_id`: The account detail id for which to retrieve the valid `yearmonth` codes. Valid `account_detail_id`s can be retrieved using the using the [GetAccountDetails](GetAccountDetails.md) call.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<account-periods>
  <yearmonth>201204</yearmonth>
  <yearmonth>201203</yearmonth>
  <yearmonth>201202</yearmonth>
  <yearmonth>201201</yearmonth>
  <yearmonth>201112</yearmonth>
  <yearmonth>201111</yearmonth>
</account-periods>
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```