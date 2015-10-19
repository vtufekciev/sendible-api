To retrieve the list of all Sendible SmartQueues for a given user, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/queues.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
    {
        "queue_times": [
            {
                "minute": 33,
                "hour": 2,
                "id": 279620,
                "weekday": 5
            },
            {
                "minute": 42,
                "hour": 2,
                "id": 279621,
                "weekday": 5
            },
            {
                "minute": 39,
                "hour": 4,
                "id": 279614,
                "weekday": 4
            },
            {
                "minute": 17,
                "hour": 6,
                "id": 279608,
                "weekday": 3
            },
            {
                "minute": 2,
                "hour": 9,
                "id": 279602,
                "weekday": 2
            },
            {
                "minute": 4,
                "hour": 9,
                "id": 279590,
                "weekday": 0
            },
            {
                "minute": 5,
                "hour": 9,
                "id": 279615,
                "weekday": 4
            },
            {
                "minute": 7,
                "hour": 9,
                "id": 279603,
                "weekday": 2
            },
            {
                "minute": 12,
                "hour": 9,
                "id": 279622,
                "weekday": 5
            },
            {
                "minute": 22,
                "hour": 9,
                "id": 279591,
                "weekday": 0
            },
            {
                "minute": 23,
                "hour": 9,
                "id": 279609,
                "weekday": 3
            },
            {
                "minute": 3,
                "hour": 10,
                "id": 279623,
                "weekday": 5
            },
            {
                "minute": 5,
                "hour": 10,
                "id": 279626,
                "weekday": 6
            },
            {
                "minute": 31,
                "hour": 10,
                "id": 279610,
                "weekday": 3
            },
            {
                "minute": 42,
                "hour": 10,
                "id": 279611,
                "weekday": 3
            },
            {
                "minute": 51,
                "hour": 10,
                "id": 279627,
                "weekday": 6
            },
            {
                "minute": 11,
                "hour": 11,
                "id": 279596,
                "weekday": 1
            },
            {
                "minute": 12,
                "hour": 11,
                "id": 279604,
                "weekday": 2
            },
            {
                "minute": 33,
                "hour": 11,
                "id": 279597,
                "weekday": 1
            },
            {
                "minute": 41,
                "hour": 11,
                "id": 279605,
                "weekday": 2
            },
            {
                "minute": 56,
                "hour": 11,
                "id": 279628,
                "weekday": 6
            },
            {
                "minute": 34,
                "hour": 12,
                "id": 279612,
                "weekday": 3
            },
            {
                "minute": 5,
                "hour": 13,
                "id": 279616,
                "weekday": 4
            },
            {
                "minute": 23,
                "hour": 13,
                "id": 279606,
                "weekday": 2
            },
            {
                "minute": 32,
                "hour": 13,
                "id": 279617,
                "weekday": 4
            },
            {
                "minute": 2,
                "hour": 15,
                "id": 279592,
                "weekday": 0
            },
            {
                "minute": 5,
                "hour": 15,
                "id": 279593,
                "weekday": 0
            },
            {
                "minute": 22,
                "hour": 15,
                "id": 279598,
                "weekday": 1
            },
            {
                "minute": 30,
                "hour": 15,
                "id": 279599,
                "weekday": 1
            },
            {
                "minute": 46,
                "hour": 16,
                "id": 279618,
                "weekday": 4
            },
            {
                "minute": 11,
                "hour": 17,
                "id": 279619,
                "weekday": 4
            },
            {
                "minute": 32,
                "hour": 17,
                "id": 279629,
                "weekday": 6
            },
            {
                "minute": 12,
                "hour": 18,
                "id": 279600,
                "weekday": 1
            },
            {
                "minute": 51,
                "hour": 18,
                "id": 279601,
                "weekday": 1
            },
            {
                "minute": 15,
                "hour": 19,
                "id": 279624,
                "weekday": 5
            },
            {
                "minute": 17,
                "hour": 19,
                "id": 279630,
                "weekday": 6
            },
            {
                "minute": 33,
                "hour": 19,
                "id": 279631,
                "weekday": 6
            },
            {
                "minute": 15,
                "hour": 20,
                "id": 279625,
                "weekday": 5
            },
            {
                "minute": 47,
                "hour": 20,
                "id": 279607,
                "weekday": 2
            },
            {
                "minute": 1,
                "hour": 21,
                "id": 279594,
                "weekday": 0
            },
            {
                "minute": 14,
                "hour": 21,
                "id": 279595,
                "weekday": 0
            },
            {
                "minute": 10,
                "hour": 22,
                "id": 279613,
                "weekday": 3
            }
        ],
        "can_repeat": 0,
        "queue_name": "My Queue",
        "id": 9,
        "user_id": 5131,
        "auto_detect": 0
    },
    {
        "queue_times": [],
        "can_repeat": 0,
        "queue_name": "test",
        "id": 132,
        "user_id": 5131,
        "auto_detect": 0
    },
    {
        "queue_times": [],
        "can_repeat": 0,
        "queue_name": "test2",
        "id": 140,
        "user_id": 5131,
        "auto_detect": 0
    },
    {
        "queue_times": [],
        "can_repeat": 0,
        "queue_name": "test3",
        "id": 143,
        "user_id": 5131,
        "auto_detect": 0
    },
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
    },
    {
        "queue_times": [
            {
                "minute": 15,
                "hour": 9,
                "id": 2976,
                "weekday": 0
            },
            {
                "minute": 15,
                "hour": 9,
                "id": 2997,
                "weekday": 6
            },
            {
                "minute": 15,
                "hour": 9,
                "id": 2994,
                "weekday": 5
            },
            {
                "minute": 15,
                "hour": 9,
                "id": 2991,
                "weekday": 4
            },
            {
                "minute": 15,
                "hour": 9,
                "id": 2988,
                "weekday": 3
            },
            {
                "minute": 15,
                "hour": 9,
                "id": 2985,
                "weekday": 2
            },
            {
                "minute": 15,
                "hour": 9,
                "id": 2982,
                "weekday": 1
            },
            {
                "minute": 8,
                "hour": 12,
                "id": 2977,
                "weekday": 0
            },
            {
                "minute": 15,
                "hour": 13,
                "id": 2983,
                "weekday": 1
            },
            {
                "minute": 15,
                "hour": 13,
                "id": 2998,
                "weekday": 6
            },
            {
                "minute": 15,
                "hour": 13,
                "id": 2986,
                "weekday": 2
            },
            {
                "minute": 15,
                "hour": 13,
                "id": 2995,
                "weekday": 5
            },
            {
                "minute": 15,
                "hour": 13,
                "id": 2992,
                "weekday": 4
            },
            {
                "minute": 15,
                "hour": 13,
                "id": 2989,
                "weekday": 3
            },
            {
                "minute": 29,
                "hour": 15,
                "id": 2979,
                "weekday": 0
            },
            {
                "minute": 21,
                "hour": 16,
                "id": 2980,
                "weekday": 0
            },
            {
                "minute": 15,
                "hour": 17,
                "id": 2990,
                "weekday": 3
            },
            {
                "minute": 15,
                "hour": 17,
                "id": 2993,
                "weekday": 4
            },
            {
                "minute": 15,
                "hour": 17,
                "id": 2978,
                "weekday": 0
            },
            {
                "minute": 15,
                "hour": 17,
                "id": 2987,
                "weekday": 2
            },
            {
                "minute": 15,
                "hour": 17,
                "id": 2996,
                "weekday": 5
            },
            {
                "minute": 15,
                "hour": 17,
                "id": 2984,
                "weekday": 1
            },
            {
                "minute": 15,
                "hour": 17,
                "id": 2999,
                "weekday": 6
            },
            {
                "minute": 11,
                "hour": 18,
                "id": 2981,
                "weekday": 0
            }
        ],
        "can_repeat": 0,
        "queue_name": "Vishal Pindoriya's Queue",
        "id": 11,
        "user_id": 96391,
        "auto_detect": 0
    }
]
```