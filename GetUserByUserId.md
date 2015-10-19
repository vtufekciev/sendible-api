To retrieve an existing user, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/user.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.

The following parameters are optional. If they are not provided, then the authenticated user's details are used.
  * `user_id`: The ID of the user to retrieve.
  * `user_api_key`: The API key of the user to retrieve.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "profile": "Team Member",
    "lineage": "122068",
    "is_active": true,
    "fullname": "Test User",
    "api_key": "c48c7db283e1d1b57f1449d1c02d6083b0e1e6a2",
    "last_login": "2013/09/25 13:59:13 +0000",
    "id": 122068,
    "color": "#000000",
    "avatar": "http://www.gravatar.com/avatar/4b13c1a4f17c731280e51faead7bc1f3?s=55&d=http://sendible.com/images/silhouette.png",
    "user_status": "Active (Premium)",
    "parent_user_id": null,
    "login": "xpxaaaaaa",
    "email": "infobbbaaa123@sendible.com",
    "permission_profile":{"profile_name":"Default","id":2},
    "manager_of": [
        {
            "user": {
              "id": 1234,
              "login": "john1",
              "fullname": "John Smith"
            }
        },
        {
            "user": {
               "id": 1235,
               "login": "john2",
              "fullname": "John Jones"
             }
        }
      ]
}
```

#### Error Responses: ####
```
{"error": {"type": "NotFound", "message": "The user could not be found."} }
```