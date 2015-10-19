To delete an existing user, make a DELETE call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/user.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `user_id`: The ID of the user to update.
  * `user_api_key`: The API key of the user to update.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "status": "OK",
}
```

#### Error Responses: ####
```
{"error": {"type": "NotFound", "message": The user could not be found."} }
```