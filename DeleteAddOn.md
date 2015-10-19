To delete an add-on, make a DELETE call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/add_ons.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `add_on_id`: The id of the add-on to be deleted.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{"status": "OK"}
```