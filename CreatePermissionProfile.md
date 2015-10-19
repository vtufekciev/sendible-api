To create a new permission profile, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/permission_profile.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `profile_name`: The name of the profile.
  * `permissions`: Optional. A comma separated list of permission IDs. This list can be retrieved using the available\_permissions API call.


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
{"error": {"type": "MissingParameter", "message": "The profile_name parameter is missing."} }
```