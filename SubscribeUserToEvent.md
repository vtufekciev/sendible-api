To create a new event subscription for the authenticated user, make a POST request. Once configured, Sendible will issue a POST with the following parameters to your callback url: `verification_code`, `object_name`, `event_name`, `data`.

#### URL: ####
http://sendible.com/api/v2/event_subscription.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `subscription_id`: Required. The specific `developer_subscription` event that the authenticated user will be subscribing to.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user that will be subscribing to the event.

#### Success Response: ####
```
{"status": "OK" }
```


#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```