To retrieve a list of the user's strean account details, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/stream-accounts.json

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
        "description": "Microsoft Corporation",
        "id": 239937,
        "service": {
            "description": "Monitor Twitter for search terms.",
            "icon": "http://twitter.com/phoenix/favicon.ico",
            "id": 1495,
            "title": "Twitter Search",
            "stream_actions": [
                {
                    "name": "Reply",
                    "action": "reply",
                    "can_message": true,
                    "message_prefix": "@"
                },
                {
                    "name": "DM",
                    "action": "dm",
                    "can_message": true,
                    "message_prefix": "d "
                },
                {
                    "name": "Retweet",
                    "action": "retweet",
                    "can_message": true,
                    "message_prefix": "RT @"
                }
            ]
        }
    }
]
```