To retrieve notifications for a user, make an authenticated GET request.

#### URL: ####
http://sendible.com/api/v2/notifications.json

#### HTTP Methods: ####
GET

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `language`: Optional. Set this to the user's language code. E.g. `en`, `es` etc.
  * `page`: Optional. Set this to the page number you would like to retrieve.
  * `per_page`: Optional. Set this to the number of results to return per page. Default is 20.


#### Success Response: ####

Currently, we have 3 types of notification:
  * `reconnect`: Shown when the user needs to reconnect a broken service. (e.g. Facebook after a password change)
  * `message`: Shown for general messages/alerts.
  * `timezone`: Shown if the user's browser timezone does not match what's stored on the server.

```
[
    {
        "created_at_local": "2014/04/10 21:23:23 +0000",
        "notification_type": "reconnect",
        "user_id": 5131,
        "title": "Facebook Reconnection Issue",
        "data": "{\"reconnection_url\": \"/services/edit/53?aid=747547&src=api\"}",
        "language": "en",
        "is_read": 0,
        "id": 3,
        "message": "We noticed that you recently changed your Facebook password. Please click here to reconnect.",
        "created_at": "2014/04/10 20:23:23 +0000",
        "avatar": "https://cdn2.iconfinder.com/data/icons/metro-ui-dock/128/Facebook_alt_1.png"
    },
    {
        "created_at_local": "2014/04/10 21:21:03 +0000",
        "notification_type": "message",
        "user_id": 5131,
        "title": "Discount Code",
        "data": "{\"url\": \"/upgrade?discount_code=x\"}",
        "language": "en",
        "is_read": 0,
        "id": 2,
        "message": "Use this discount code and save 15%!",
        "created_at": "2014/04/10 20:21:03 +0000",
        "avatar": "https://cdn2.iconfinder.com/data/icons/metro-ui-dock/128/Email_Chat.png"
    },
    {
        "created_at_local": "2014/04/10 21:19:27 +0000",
        "notification_type": "timezone",
        "user_id": 5131,
        "title": "Timezone Mismatch",
        "data": "{}",
        "language": "en",
        "is_read": 0,
        "id": 1,
        "message": "We noticed that your local timezone is different from the timezone on your account. ",
        "created_at": "2014/04/10 20:19:27 +0000",
        "avatar": "https://cdn1.iconfinder.com/data/icons/metro-ui-dock/128/Clock.png"
    }
]
```