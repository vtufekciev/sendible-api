To create a new event subscription for your application, make a POST request.

#### URL: ####
http://sendible.com/api/v2/developer_subscription.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `object_name`: Required. Valid values are `Contact`, `SMSIn`.
  * `event_name`: Required. Valid values are `Create`, `Update`, `Delete`.
  * `verification_code`: Required. This parameter and value will be passed to your callback URL for verification.
  * `callback_url`: Required. This is the URL that Sendible will POST to when the event fires.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "object_name": "Contact",
    "callback_url": "http://myurl.com",
    "subscribers": [],
    "id": 1,
    "event_name": "Create",
    "verification_code": "test123"
}
```


#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```