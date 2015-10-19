To retrieve a user's list of services used by the Priority Inbox (for filtering purposes), make a GET request.

#### URL: ####
http://sendible.com/api/v2/inbox_services.json

#### HTTP Methods: ####
GET

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.

#### Success Response: ####
```
[
    {
        "description": "YouTube",
        "picture_url": "https://i3.ytimg.com/i/j80sc-d9NXS43a6FGXHBVQ/1.jpg?v=4f0c620c",
        "id": 1112,
        "account_name": "sendible"
    },
    {
        "description": "Twitter",
        "picture_url": "http://pbs.twimg.com/profile_images/435435959669096449/rA7jKuts_normal.png",
        "id": 1223,
        "account_name": "Sendible"
    },
    {
        "description": "Facebook Fan Page",
        "picture_url": "http://graph.facebook.com/21274802454/picture",
        "id": 1235,
        "account_name": "Sendible"
    }
]
```