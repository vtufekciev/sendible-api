To delete a permission profile, make a DELETE call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/permission_profile.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `profile_id`: The ID of the profile to delete.


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "status": "OK"
}
```

#### Error Responses: ####
```
{"error": {"type": "MissingParameter", "message": "The profile_id parameter is missing."} }
```