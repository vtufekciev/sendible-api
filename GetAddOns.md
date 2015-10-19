To retrieve a user's purchased add-ons, make an authenticated GET request.

#### URL: ####
http://sendible.com/api/v2/add_ons.json

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
        "amount": 0,
        "sms_price_id": 302,
        "id": 820,
        "currency": "",
        "created_at": "2013/06/26 18:06:49 +0000",
        "user_id": 115727,
        "frequency": 0,
        "item_name": "Rebranding - via GetSync'd",
        "completed": 1,
        "updated_at": "2013/06/26 18:06:49 +0000",
        "notes": "Rebranding: via GetSync'd, Website: http://www.getsyncd.com, User_id: 115727"
    },
    {
        "amount": 0,
        "sms_price_id": 263,
        "id": 434,
        "currency": "",
        "created_at": "2012/10/16 14:43:30 +0000",
        "user_id": 96391,
        "frequency": 0,
        "item_name": "Rebranding - via VishalPindoriya",
        "completed": 1,
        "updated_at": "2012/10/16 14:43:30 +0000",
        "notes": "Rebranding: via VishalPindoriya, Website: http://www.facebook.com/v.pindoriya, User_id: 96391"
    }
]
```