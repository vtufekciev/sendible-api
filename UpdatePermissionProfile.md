To update a permission profile, make a PUT call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/permission_profile.json

#### HTTP Methods: ####
PUT

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `profile_id`: The ID of the profile to update.
  * `profile_name`: The name of the profile to update.


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "profile_name": "Default 3",
    "id": 4,
    "permissions": []
}
```

#### Error Responses: ####
```
{"error": {"type": "MissingParameter", "message": "The profile_id parameter is missing."} }
```

```
{"error": {"type": "MissingParameter", "message": "The profile_name parameter is missing."} }
```