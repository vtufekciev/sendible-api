To update a notification for a user, make an authenticated PUT request.

#### URL: ####
http://sendible.com/api/v2/notifications.json

#### HTTP Methods: ####
PUT

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `notification_id`: The id or id's of the notification(s) to update. To update multiple notifications at once, separate the notification\_id's with commas.
  * `is_read`: Set to 1 if the notification has been read or 0 otherwise. Note:

#### Success Response: ####
```
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
```