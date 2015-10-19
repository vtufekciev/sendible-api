To create a new user, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/user.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `fullname`: The name of the user.
  * `email`: The email address of the user.
  * `login`: The username of the user.
  * `password`: The password of the user.
  * `profile`: Either `administrator`, `team member` or `client`.
  * `timezone`: Optional. The user's timezone offset from GMT in minutes. Default: The admin user's timezone will be used. In Javascript, this is the value of `getTimezoneOffset`.
  * `managed_by_id`: Optional. The user ID of the user that manages this user. Default: None.
  * `approval_from_ids`: Optional. A comma-separated list of user ID's that need to approve this user's content before it is published.
  * `permission_profile_id`: Optional. The permission profile ID to set for the user.
  * `manager_of`: Optional. A comma separated list of user IDs that this user can manage.


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
    "email": "infobbbaaa123@sendible.com"
}
```

#### Error Responses: ####
```
{"error": {"type": "MissingParameter", "message": "The profile parameter is missing."} }
```

```
{"error": {"type": "InvalidUsername", "message": "This username is already in use."} }
```

```
{"error": {"type": "InvalidUsername", "message": "This email is already in use."} }
```

```
{"error": {"type": "InvalidUsername", "message": "Username must be longer than 3 characters."} }
```