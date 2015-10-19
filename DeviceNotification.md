To send a push notification to mobile device, make a POST request, authenticating as the user. This will send a push notification to all devices registered to the authenticating user.

#### URL: ####
http://sendible.com/api/v2/device_notification.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `message`: Required. The message that will be sent to the device. This needs to be a JSON message.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Response: ####
```
{
    {
    "success": [
        {
            "last_error": "InvalidRegistration",
            "device_type": "android",
            "device_id": "12345"
        }
     ],
    "failed": [
        {
            "last_error": "InvalidRegistration",
            "device_type": "android",
            "device_id": "999"
        }
    ]
}
}
```