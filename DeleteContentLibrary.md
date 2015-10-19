To delete a content library, make a DELETE call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/content_library.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `id`: The id of the library to be deleted.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
   "status": "OK"
}
```