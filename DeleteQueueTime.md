To delete one of the times on a SmartQueue, make a DELETE call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/queue_times.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `queue_time_id`: The id belonging to the SmartQueue time item.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{"status": "OK"}
```