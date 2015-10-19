To create a new custom field, make a POST request.

#### URL: ####
http://sendible.com/api/v2/custom_field.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `field_title`: The field title.
  * `category`: The custom field category. Either: `user`, `contact` or `account`.
  * `field_type`: The type of field. Either: `text`, `textarea`, `password`, `list`, `date`, `time`, `url`, `numeric`.
  * `sort_order`: A numeric value representing the order that this field appears in.
  * `mandatory`: Specifies whether this field is mandator or not. `1` or `0`.
  * `field_options`: When `field_type` is `list`, this represents a list of options. Each option in the list is separated by a line break.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
    {
        "created_at": "2012/04/27 16:03:02 +0000",
        "category": "user",
        "whitelabel": "Sendible Team",
        "updated_at": "2012/04/27 16:03:02 +0000",
        "field_value": "",
        "sort_order": 1,
        "mandatory": 1,
        "id": 32772,
        "user_id": 5131,
        "field_options": "New York\nLos Angeles",
        "field_type": "list",
        "field_name": "city",
        "field_title": "City"
    },
    {
        "created_at": "2012/04/19 12:35:03 +0000",
        "category": "user",
        "whitelabel": "Sendible Team",
        "updated_at": "2012/04/19 12:35:03 +0000",
        "field_value": "",
        "sort_order": 1,
        "mandatory": 1,
        "id": 31660,
        "user_id": 59119,
        "field_options": "",
        "field_type": "text",
        "field_name": "field3",
        "field_title": "Field3"
    },
    {
        "created_at": "2012/04/19 07:51:35 +0000",
        "category": "user",
        "whitelabel": "Sendible Team",
        "updated_at": "2012/04/19 07:51:35 +0000",
        "field_value": "",
        "sort_order": 1,
        "mandatory": 1,
        "id": 31656,
        "user_id": 5131,
        "field_options": "Melbourne\nSydney",
        "field_type": "list",
        "field_name": "location",
        "field_title": "Location"
    },
    {
        "created_at": "2012/05/11 15:24:27 +0000",
        "category": "user",
        "whitelabel": "Sendible Team",
        "updated_at": "2012/05/11 15:24:27 +0000",
        "field_value": "",
        "sort_order": 1,
        "mandatory": 1,
        "id": 33554,
        "user_id": 5131,
        "field_options": "",
        "field_type": "text",
        "field_name": "neighbourhood",
        "field_title": "neighbourhood"
    },
    {
        "created_at": "2012/10/24 10:56:38 +0000",
        "category": "user",
        "whitelabel": "Sendible Team",
        "updated_at": "2012/10/24 10:56:38 +0000",
        "field_value": "",
        "sort_order": 1,
        "mandatory": 0,
        "id": 51348,
        "user_id": 77515,
        "field_options": "",
        "field_type": "text",
        "field_name": "signature",
        "field_title": "Signature"
    },
    {
        "created_at": "2012/04/25 15:12:02 +0000",
        "category": "user",
        "whitelabel": "Sendible Team",
        "updated_at": "2012/04/25 15:12:02 +0000",
        "field_value": "",
        "sort_order": 1,
        "mandatory": 1,
        "id": 32184,
        "user_id": 5131,
        "field_options": "Store 1\nStore 2\n",
        "field_type": "list",
        "field_name": "store_name",
        "field_title": "store name"
    },
    {
        "created_at": "2012/10/16 17:00:58 +0000",
        "category": "user",
        "whitelabel": "Sendible Team",
        "updated_at": "2012/10/16 17:00:58 +0000",
        "field_value": "",
        "sort_order": 1,
        "mandatory": 0,
        "id": 50968,
        "user_id": 5131,
        "field_options": "",
        "field_type": "text",
        "field_name": "twitter_hashtag",
        "field_title": "Twitter Hashtag"
    },
    {
        "created_at": "2012/10/16 16:58:16 +0000",
        "category": "user",
        "whitelabel": "Sendible Team",
        "updated_at": "2012/10/16 16:58:16 +0000",
        "field_value": "",
        "sort_order": 1,
        "mandatory": 0,
        "id": 50967,
        "user_id": 5131,
        "field_options": "",
        "field_type": "password",
        "field_name": "twitter_password",
        "field_title": "Twitter Password"
    }
]
```


#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```