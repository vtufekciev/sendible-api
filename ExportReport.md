Returns a downloadable HTML or CSV report for all account data for a given period. Make a GET call using the api key of the authenticated user.

#### URL: ####
http://sendible.com/reports?type=account-report&ext=format

#### Formats: ####
Replace `format` with either `html` or `csv`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `access_key`: The `api_key` belonging to the authenticated user.
  * `account_detail_id`: The account detail id for which to retrieve the valid `yearmonth` codes.
  * `yearmonth`: The `yearmonth` period for which to export.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
A downloadable file in the specified format of HTML or CSV.
```