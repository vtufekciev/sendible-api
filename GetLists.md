To retrieve lists of services for a given user, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/lists.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `type`: Optional. `all`, `owner`, `contributor` or `consumer`.
  * `list_type`: Optional. `mixed`, `social`, `sms` or `email`. To filter by multiple list types, separate with commas. E.g. `sms`,`email`.
  * `per_page`: Optional. The number of lists to return per page.
  * `page`: Optional. The page number to return.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
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
        "item_count": 0,
        "list_type": "Social",
        "list_name": "My List"
    },
    {
        "consumers": [],
        "contributors": [],
        "id": 630,
        "user_id": 5131,
        "item_count": 2,
        "list_type": "Social",
        "list_name": "Sendible Twitter"
    },
    {
        "consumers": [],
        "contributors": [],
        "id": 9631,
        "user_id": 5131,
        "item_count": 0,
        "list_type": "Social",
        "list_name": "Twitter and Facebook"
    }
]
```