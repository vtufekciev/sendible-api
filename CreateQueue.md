To create or Sendible SmartQueue for a given user, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/queue.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `queue_name`: The name of the queue.
  * `auto_detect`: This is not currently in use. Please use 0.
  * `can_repeat`:  This is not currently in use. Please use 0.
  * `contributors`:  Optional. A comma separated lists of user IDs representing users that can contribute to this queue.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "queue_times": [],
    "can_repeat": 0,
    "queue_name": "My Queue",
    "id": 9004,
    "user_id": 5131,
    "auto_detect": 0
}
```