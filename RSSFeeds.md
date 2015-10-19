Retrieve the authenticated user's RSS Feeds.

#### URL: ####
http://sendible.com/api/v2/rssfeeds.json

#### HTTP Methods: ####
GET

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.

#### Success Response: ####
```
[
    {
        "feed_url": "http://feeds.mashable.com/Mashable",
        "id": 1,
        "feed_name": "Mashable",
        "user_id": 5131,
        "created_at": "2010/01/21 14:36:11 +0000"
    },
    {
        "feed_url": "http://social-media.alltop.com/rss/",
        "id": 5,
        "feed_name": "Social Media Alltop",
        "user_id": 5131,
        "created_at": "2010/01/21 14:44:12 +0000"
    },
    {
        "feed_url": "http://webworkerdaily.com/feed/",
        "id": 6,
        "feed_name": "Web Worker Daily",
        "user_id": 5131,
        "created_at": "2010/01/22 09:09:23 +0000"
    },
    {
        "feed_url": "http://gavin.sendible.com/rss.xml",
        "id": 20,
        "feed_name": "Gavin's blog",
        "user_id": 5131,
        "created_at": "2010/02/12 11:52:40 +0000"
    },
    {
        "feed_url": "http://feeds.feedburner.com/readwriteweb",
        "id": 21,
        "feed_name": "RWW",
        "user_id": 5131,
        "created_at": "2010/02/16 13:42:48 +0000"
    },
    {
        "feed_url": "http://www.amazon.co.uk/rss/bestsellers/books/?tag=sendible-21",
        "id": 37,
        "feed_name": "Amazon Books Bestsellers",
        "user_id": 5131,
        "created_at": "2010/02/27 13:36:38 +0000"
    },
    {
        "feed_url": "http://www.amazon.co.uk/rss/bestsellers/electronics?tag=sendible-21",
        "id": 38,
        "feed_name": "Amazon Electronics Bestsellers",
        "user_id": 5131,
        "created_at": "2010/02/27 13:41:17 +0000"
    },
    {
        "feed_url": "http://www.amazon.co.uk/rss/bestsellers/videogames?tag=sendible-21",
        "id": 39,
        "feed_name": "Amazon Videogames Bestsellers",
        "user_id": 5131,
        "created_at": "2010/02/27 13:43:43 +0000"
    }
]
```

#### Error Response: ####
```
{{
    "error": {
        "type": "InvalidHTTPMethod",
        "message": "PUTisinvalidforthisendpoint."
    }
}
```