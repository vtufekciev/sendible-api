To delete the user's Sendible SmartQueue, make a DELETE call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/queue.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `queue_id`: The id belonging to the SmartQueue.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{"status": "OK"}
```