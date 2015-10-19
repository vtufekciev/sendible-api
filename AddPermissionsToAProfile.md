To specify all permissions for a permission profile, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/permissions.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `profile_id`: The ID of the profile to retrieve.
  * `permissions`: A comma separated list of permission IDs. This list can be retrieved using the `available_permissions` API call.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "profile_name": "Default",
    "id": 2,
    "permissions": [
        {
            "permission_category": {
                "category_name": "Engage",
                "id": 1,
                "sorting": 1
            },
            "permission_description": "The user can compose new messages.",
            "id": 2,
            "permission_name": "Compose Messages",
            "permission_code": "messages.create"
        }
    ]
}
```

#### Error Responses: ####
```
{"error": {"type": "MissingParameter", "message": "The profile_id parameter is missing."} }
```

```
{"error": {"type": "MissingParameter", "message": "The permissions parameter is missing."} }
```