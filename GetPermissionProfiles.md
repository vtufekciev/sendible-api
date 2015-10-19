To retrieve all available permission profiles make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/permission_profiles.json

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
        "profile_name": "Default",
        "id": 2
    },
    {
        "profile_name": "Default 2",
        "id": 3
    }
]
```