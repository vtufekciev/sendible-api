To retrieve a the profile for an authenticated user, make a GET call using an access\_token.

#### URL: ####
http://sendible.com/api/v2/profile.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `timezone`: Optional. Pass the timezoneOffsetClient value from the browser. This will be used to determine if the user's browser timezone differs from that in their profile preferences.

#### Authentication: ####
Use the access\_token that's retrieved after a call to http://sendible.com/api/v2/auth.

#### Success Response: ####
```
{
    "permission_profile": {
        "profile_name": "Default",
        "id": 2,
        "permissions": [
            {
                "permission_id": "1",
                "permission_description": "The user can compose new messages.",
                "permission_name": "Compose Messages",
                "permission_code": "messages.create",
                "permission_category": {
                    "category_name": "Engage",
                    "id": 1,
                    "sorting": 1
                }
            }
        ]
    },
    "approval_from": [],
    "profile": "Administrator",
    "is_active": true,
    "lineage": "1234",
    "children_count": 4,
    "last_login": "2013/10/08 09:05:41 +0000",
    "user_status": "Active (Premium)",
    "language": "en",
    "fullname": "John Smith",
    "api_key": "xxxxxxxxxxxxxx",
    "timezone": -60,
    "id": 1234,
    "color": "#b6617c",
    "user_properties": [
        {
            "created_at": "2013/02/26 00:00:00 +0000",
            "updated_at": "2013/02/26 18:18:42 +0000",
            "propertyName": "google_fonts",
            "id": 422,
            "user_id": 5131,
            "propertyValue": "{\"items\":[]}"
        }
    ],
    "timezone_name": "Europe - London",
    "mobile": "",
    "parent_user_id": null,
    "login": "sendible",
    "company_address": "",
    "avatar": "https://s3.amazonaws.com/files.sendible.com/135875/thumb.png",
    "email": "info@xxxx.xxxx",
    "clock_format": 12
}
```