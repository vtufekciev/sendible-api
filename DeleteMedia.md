To delete a media file for a given user, make a DELETE call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/media.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `file_id`: The id of the file to be deleted.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
   "status": "OK"
}
```