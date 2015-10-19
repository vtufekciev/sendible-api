To retrieve an existing content library, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/content_library.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `content_library_id`: The id of the content library to retrieve.

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