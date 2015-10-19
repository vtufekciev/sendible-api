To share an account (service) with other users, make a POST request.

#### URL: ####
http://sendible.com/api/v2/account_shares.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_id`: The account id.
  * `contributors`: A comma separated list of user ID's to share the service with.

#### Authentication: ####
Basic authentication with username and password or remote API key/access token belonging to the Sendible user.

#### Success Response: ####
```
{"status": "OK" }
```