To retrieve a list of all active event subscriptions for your application, make a GET request.

#### URL: ####
http://sendible.com/api/v2/developer_subscriptions.json

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
        "object_name": "Contact",
        "callback_url": "http://myurl.com",
        "subscribers": [
            {
                "user": {
                    "fullname": "John Smith",
                    "api_key": "**********",
                    "login": "sendible",
                    "email": "**@****.***"
                },
                "id": 1
            }
        ],
        "id": 1,
        "event_name": "Create",
        "verification_code": "test123"
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