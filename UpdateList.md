To update an existing list, make a PUT call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/list.json

#### HTTP Methods: ####
PUT

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `list_id`: The id of the list to update.
  * `list_name`: The name of the list.
  * `consumers`: A comma separated list of user ID's that can post using this list. User `ALL` to add all team members/users this user manages.
  * `contributors`: A comma separated list of user ID's that can add services to this list. User `ALL` to add all team members/users this user manages.
  * `color`: Optional. The color for the list.


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "consumers": [
        {
            "user": {
                "fullname": "Ankit Shah",
                "id": 59119,
                "color": "#8694e9",
                "login": "anky"
            },
            "id": 47629
        },
        {
            "user": {
                "fullname": "Johnny Costello",
                "id": 77515,
                "color": "#af1c22",
                "login": "johnny"
            },
            "id": 47630
        }
    ],
    "contributors": [
        {
            "user": {
                "fullname": "Ankit Shah",
                "id": 59119,
                "color": "#8694e9",
                "login": "anky"
            },
            "id": 47631
        },
        {
            "user": {
                "fullname": "Johnny Costello",
                "id": 77515,
                "color": "#af1c22",
                "login": "johnny"
            },
            "id": 47632
        }
    ],
    "id": 47925,
    "user_id": 5131,
    "list_type": "Social",
    "list_name": "My List"
}
```