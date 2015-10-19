To retrieve the list of all available permission categories make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/permission_categories.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
    {
        "category_name": "Engage",
        "id": 1,
        "sorting": 1,
        "category_description": "Permissions for the Engage Tab"
    }
]
```