To delete an application subscription, make a DELETE request.

#### URL: ####
http://sendible.com/api/v2/developer_subscription.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `subscription_id`: The id for one of your previously created subscriptions.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

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