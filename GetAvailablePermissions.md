To retrieve the list of all available permissions make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/available_permissions.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `category_id`: Optional. The category of permissions to retrieve. To retrieve the categories, use the `permission_categories` API endpoint.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
    {
        "permission_category": {
            "category_name": "Engage",
            "id": 1,
            "sorting": 1,
            "category_description": "Permissions for the Engage Tab"
        },
        "permission_description": "The user can compose new messages.",
        "id": 1,
        "permission_name": "Compose Messages",
        "permission_code": "messages.create"
    }
]
```