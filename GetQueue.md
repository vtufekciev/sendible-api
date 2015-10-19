To retrieve a given Sendible SmartQueue, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/queue.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `queue_id`: The id belonging to the SmartQueue.

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