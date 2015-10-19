To update receipt details such as VAT number and billing email addresses for an account, make a PUT request.

#### URL: ####
http://sendible.com/api/v2/receipts.json

#### HTTP Methods: ####
PUT

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `vat_number`: The VAT number provided by the user.
  * `billing_email`: A comma separated list of email addresses.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "status": "OK"
}
```