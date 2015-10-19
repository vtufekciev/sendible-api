To create or Sendible SmartQueue for a given user, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/queue.json

#### HTTP Methods: ####
PUT

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `queue_id`: The id of the queue to update.
  * `queue_name`: Optional. The name of the queue.
  * `queue_times`: Optional. The comma separated list of queue times. These will replace the existing ones on the queue. In the format, `day_index`|`hour`|`minute`,`day_index`|`hour`|`minute`,....,`day_index`|`hour`|`minute`
day\_index of 0 represents Monday. day\_index of 6 is Sunday.
For example: 0|11|30,2|14|44 represents: Monday at 11.30, Wednesday at 2.44pm.
  * `contributors`:  Optional. A comma separated lists of user IDs representing users that can contribute to this queue.
  * `can_repeat`:  Please use 1 if messages can repeat, otherwise 1.


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "queue_times": [
        {
            "minute": 30,
            "hour": 11,
            "id": 284406,
            "weekday": 0
        },
        {
            "minute": 44,
            "hour": 14,
            "id": 284407,
            "weekday": 2
        }
    ],
    "can_repeat": 0,
    "queue_name": "My Queue",
    "id": 9004,
    "user_id": 5131,
    "auto_detect": 0
}
```