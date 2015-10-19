To create a new content library, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/content_library.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `library_name`: The name of the library.
  * `consumers`: A comma separated list of user ID's that can consume content in this library. User `ALL` to add all team members/users this user manages.
  * `contributors`: A comma separated list of user ID's that can contribute content to this library. User `ALL` to add all team members/users this user manages.


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "created_at": "2013/08/29 11:39:16 +0000",
    "consumers": [
        {
            "user": {
                "fullname": "Gavin Hammar",
                "id": 5131,
                "color": "#b6617c",
                "login": "sendible"
            },
            "id": 46737
        },
        {
            "user": {
                "fullname": "Sendible.com1",
                "id": 1,
                "color": "#d79d54",
                "login": "hamgav"
            },
            "id": 46738
        }
    ],
    "content_type": "Message",
    "contributors": [],
    "updated_at": "2013/08/29 11:39:16 +0000",
    "id": 6,
    "user_id": 5131,
    "library_name": "Quotes"
}
```