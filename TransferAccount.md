To transfer an account (service), make a POST request.

#### URL: ####
http://sendible.com/api/v2/account_transfer.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_id`: The account id.
  * `to_user_id`: The user id to transfer the account to.

#### Authentication: ####
Basic authentication with username and password or remote API key/access token belonging to the Sendible user.

#### Success Response: ####
```
{"status": "OK" }
```