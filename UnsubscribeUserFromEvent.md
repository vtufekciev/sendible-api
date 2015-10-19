To unsubscribe the authenticated user from a subscription, make a DELETE request.

#### URL: ####
http://sendible.com/api/v2/event_subscription.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `subscription_id`: Required. The specific `developer_subscription` event that the authenticated user will be subscribing to.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user that will be unsubscribing from this event.

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