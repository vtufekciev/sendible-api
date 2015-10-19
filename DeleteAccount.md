To delete an account (service), make a DELETE request.

#### URL: ####
http://sendible.com/api/v2/account.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_id`: The account id.


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{"status": "OK" }
```