To add a new time to a given Sendible SmartQueue, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/queue_times.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `queue_id`: The id belonging to the SmartQueue.
  * `weekday`: The index of the weekday. 0 = Monday, 6 = Sunday
  * `hour`: The hour (military time format).
  * `minute`: The minute.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
        "queue_times": [
            {
                "minute": 0,
                "hour": 12,
                "id": 284406,
                "weekday": 0
            },
            {
                "minute": 0,
                "hour": 12,
                "id": 284407,
                "weekday": 2
            }
        ],
        "can_repeat": 0,
        "queue_name": "ignore",
        "id": 9004,
        "user_id": 5131,
        "auto_detect": 0
    }
```