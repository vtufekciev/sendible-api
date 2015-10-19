To retrieve the list of all Content Libraries for a given user, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/content_libraries.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `type`: Optional. `all`, `owner`, `contributor` or `consumer`.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
    {
        "created_at": "2013/08/29 10:18:04 +0000",
        "consumers": [],
        "content_type": "Message",
        "contributors": [],
        "updated_at": "2013/08/29 10:18:04 +0000",
        "id": 2,
        "user_id": 5131,
        "library_name": "My Content"
    },
    {
        "created_at": "2013/08/29 11:21:42 +0000",
        "consumers": [],
        "content_type": "Message",
        "contributors": [],
        "updated_at": "2013/08/29 11:21:42 +0000",
        "id": 3,
        "user_id": 5131,
        "library_name": "Quotes"
    },
    {
        "created_at": "2013/08/29 11:22:22 +0000",
        "consumers": [],
        "content_type": "Message",
        "contributors": [],
        "updated_at": "2013/08/29 11:22:22 +0000",
        "id": 4,
        "user_id": 5131,
        "library_name": "Quotes"
    },
    {
        "created_at": "2013/08/29 11:36:56 +0000",
        "consumers": [
            {
                "created_at": "2013/08/29 11:36:56 +0000",
                "user": {
                    "fullname": "Gavin Hammar",
                    "id": 5131,
                    "color": "#b6617c",
                    "login": "sendible"
                },
                "id": 46736
            }
        ],
        "content_type": "Message",
        "contributors": [],
        "updated_at": "2013/08/29 11:36:56 +0000",
        "id": 5,
        "user_id": 5131,
        "library_name": "Quotes"
    },
    {
        "created_at": "2013/08/29 11:39:16 +0000",
        "consumers": [
            {
                "created_at": "2013/08/29 11:39:17 +0000",
                "user": {
                    "fullname": "Gavin Hammar",
                    "id": 5131,
                    "color": "#b6617c",
                    "login": "sendible"
                },
                "id": 46737
            },
            {
                "created_at": "2013/08/29 11:39:17 +0000",
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
    },
    {
        "consumers": [
            {
                "created_at": "2013/08/29 11:36:56 +0000",
                "user": {
                    "fullname": "Gavin Hammar",
                    "id": 5131,
                    "color": "#b6617c",
                    "login": "sendible"
                },
                "id": 46736
            }
        ],
        "contributors": [],
        "id": 5,
        "user_id": 5131,
        "library_name": "Quotes (Gavin Hammar)"
    },
    {
        "consumers": [
            {
                "created_at": "2013/08/29 11:39:17 +0000",
                "user": {
                    "fullname": "Gavin Hammar",
                    "id": 5131,
                    "color": "#b6617c",
                    "login": "sendible"
                },
                "id": 46737
            },
            {
                "created_at": "2013/08/29 11:39:17 +0000",
                "user": {
                    "fullname": "Sendible.com1",
                    "id": 1,
                    "color": "#d79d54",
                    "login": "hamgav"
                },
                "id": 46738
            }
        ],
        "contributors": [],
        "id": 6,
        "user_id": 5131,
        "library_name": "Quotes (Gavin Hammar)"
    }
]
```