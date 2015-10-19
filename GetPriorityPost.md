To retrieve a single priority inbox item, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/priority-post.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `priority_post_id`: The ID of the priority post.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "responder_avatar": "http://pbs.twimg.com/profile_images/1642138996/Twitter_Icon_normal.jpg",
    "original_message": null,
    "id": 75297956,
    "service_image": "http://twitter.com/phoenix/favicon.ico",
    "message_text": "",
    "account_avatar": "http://pbs.twimg.com/profile_images/3667750807/0d1114cb36f85b8b49e45bacf9bcc485_normal.png",
    "uid": "KRSMConsulting",
    "user_id": 5131,
    "message_html": "",
    "responder_fullname": "KRSM Consulting",
    "post_picture": null,
    "responder_identifier": "@KRSMConsulting",
    "account_detail": {
        "uid": "sendible",
        "description": "Twitter",
        "account": {
            "service": {
                "icon": "http://snd-assets.s3.amazonaws.com/icons/somicro/twitter.png",
                "reply_via_filter": "twitteroauth",
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
                    },
                    {
                        "name": "Show%20Conversation",
                        "action": "sc",
                        "can_message": false,
                        "message_prefix": ""
                    },
                    {
                        "name": "Favorite",
                        "action": "favorite",
                        "can_message": false,
                        "message_prefix": ""
                    }
                ]
            }
        },
        "picture_url": "http://pbs.twimg.com/profile_images/435435959669096449/rA7jKuts_normal.png",
        "url": "http://twitter.com/Sendible",
        "account_name": "Sendible",
        "account_id": 500437
    },
    "url": "http://twitter.com/KRSMConsulting",
    "account_name": "Sendible",
    "relative_created_at": "1 month ago",
    "post_link": null,
    "isRead": 1,
    "created_at": "2014/02/13 13:03:16 +0000",
    "sentiment": 0,
    "response_type": "Mention",
    "post_body": "The KRSM Consulting Daily is out! http://t.co/hPYZCB3pRJ Stories via @Sendible @CharlieCurve",
    "service_name": "twitteroauth",
    "message_type": "Post",
    "account_detail_id": 5103
}
```