To retrieve the list of all Queue Times for a given Sendible SmartQueue, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/queue_times.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `queue_id`: The id belonging to the SmartQueue.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
    {
        "minute": 15,
        "hour": 9,
        "id": 2976,
        "queue_id": 11,
        "weekday": 0
    },
    {
        "minute": 8,
        "hour": 12,
        "id": 2977,
        "queue_id": 11,
        "weekday": 0
    },
    {
        "minute": 15,
        "hour": 17,
        "id": 2978,
        "queue_id": 11,
        "weekday": 0
    },
    {
        "minute": 29,
        "hour": 15,
        "id": 2979,
        "queue_id": 11,
        "weekday": 0
    },
    {
        "minute": 21,
        "hour": 16,
        "id": 2980,
        "queue_id": 11,
        "weekday": 0
    },
    {
        "minute": 11,
        "hour": 18,
        "id": 2981,
        "queue_id": 11,
        "weekday": 0
    },
    {
        "minute": 15,
        "hour": 9,
        "id": 2982,
        "queue_id": 11,
        "weekday": 1
    },
    {
        "minute": 15,
        "hour": 13,
        "id": 2983,
        "queue_id": 11,
        "weekday": 1
    },
    {
        "minute": 15,
        "hour": 17,
        "id": 2984,
        "queue_id": 11,
        "weekday": 1
    },
    {
        "minute": 15,
        "hour": 9,
        "id": 2985,
        "queue_id": 11,
        "weekday": 2
    },
    {
        "minute": 15,
        "hour": 13,
        "id": 2986,
        "queue_id": 11,
        "weekday": 2
    },
    {
        "minute": 15,
        "hour": 17,
        "id": 2987,
        "queue_id": 11,
        "weekday": 2
    },
    {
        "minute": 15,
        "hour": 9,
        "id": 2988,
        "queue_id": 11,
        "weekday": 3
    },
    {
        "minute": 15,
        "hour": 13,
        "id": 2989,
        "queue_id": 11,
        "weekday": 3
    },
    {
        "minute": 15,
        "hour": 17,
        "id": 2990,
        "queue_id": 11,
        "weekday": 3
    },
    {
        "minute": 15,
        "hour": 9,
        "id": 2991,
        "queue_id": 11,
        "weekday": 4
    },
    {
        "minute": 15,
        "hour": 13,
        "id": 2992,
        "queue_id": 11,
        "weekday": 4
    },
    {
        "minute": 15,
        "hour": 17,
        "id": 2993,
        "queue_id": 11,
        "weekday": 4
    },
    {
        "minute": 15,
        "hour": 9,
        "id": 2994,
        "queue_id": 11,
        "weekday": 5
    },
    {
        "minute": 15,
        "hour": 13,
        "id": 2995,
        "queue_id": 11,
        "weekday": 5
    },
    {
        "minute": 15,
        "hour": 17,
        "id": 2996,
        "queue_id": 11,
        "weekday": 5
    },
    {
        "minute": 15,
        "hour": 9,
        "id": 2997,
        "queue_id": 11,
        "weekday": 6
    },
    {
        "minute": 15,
        "hour": 13,
        "id": 2998,
        "queue_id": 11,
        "weekday": 6
    },
    {
        "minute": 15,
        "hour": 17,
        "id": 2999,
        "queue_id": 11,
        "weekday": 6
    }
]
```