To register a new mobile device for PUSH notifications, make a POST request, authenticating as the user.

#### URL: ####
http://sendible.com/api/v2/device_registration.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `device_id`: Required. The device registration ID, provided by Google or Apple.
  * `device_type`: Required. Either `android` or `ios`.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "status": "OK"
}
```