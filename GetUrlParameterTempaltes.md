Retrieve the list of URL parameter templates for the authenticated user.

#### URL: ####
http://sendible.com/api/v2/url_parameter_templates.json

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
        "user_id": 5131,
        "always_use": 0,
        "querystring": "utm_source=test",
        "preset_name": "Custom GA",
        "cannot_delete": 0,
        "id": 2
    },
    {
        "user_id": 5131,
        "always_use": 0,
        "querystring": "utm_source=&utm_medium=&utm_campaign=",
        "preset_name": "Google Analytics",
        "cannot_delete": 1,
        "id": 1
    }
]
```