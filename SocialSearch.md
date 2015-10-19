To retrieve a list of results from a realtime search on social media. Make a **GET** call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/social_search

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `type`: The type of search to perform. Possible values are `twitter` and `facebook`.
  * `query`: Search query, in text form.
  * `results_per_page`: Optional. Results to show on each page (maximum of 100)
  * `max_id`: Optional. Show only results up to this ID, used to see older results. Use the `max_id` that's returned in the results to fetch the next page of results.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.



#### Success Response: ####
```
{
    "results": [
        {
            "userimage": "https://graph.facebook.com/749169125/picture",
            "userlink": "https://facebook.com/749169125",
            "link": "https://facebook.com/749169125",
            "created_at_client": "2014-06-07T00:16:36+0000",
            "source": "facebook",
            "sentiment": 0,
            "content": "",
            "id": "1495153850697452_1498552240357613",
            "term": "sendible",
            "favicon": "http://www.google.com/s2/favicons?domain=facebook.com",
            "description": "",
            "username": "Brandon Drazic",
            "type": "facebooksearch",
            "domain": "facebook.com",
            "title": "and some positive XD\n\nhttps://www.youtube.com/watch?v=ybgKvm2KIa8&feature=youtube_gdata&utm_source=rss&utm_medium=sendible&utm_campaign=RSS",
            "nextpage": "1402010570"
        },
        {
            "userimage": "https://graph.facebook.com/21274802454/picture",
            "userlink": "https://facebook.com/21274802454",
            "link": "https://facebook.com/21274802454",
            "created_at_client": "2014-06-06T21:29:52+0000",
            "source": "facebook",
            "sentiment": 0,
            "content": "",
            "id": "21274802454_10152075828387455",
            "term": "sendible",
            "favicon": "http://www.google.com/s2/favicons?domain=facebook.com",
            "description": "",
            "username": "Sendible",
            "type": "facebooksearch",
            "domain": "facebook.com",
            "title": "Hi all\n\nWe had a very short downtime earlier but things should be back to normal now. Our server that handles user sessions failed earlier but has now been restored.\n\nWe apologise for the short downtime, but we have now corrected the issues to ensure it doesn't happen again. We generally have a 99.97% uptime, so this is extremely unusual for Sendible and we have now introduced measures to prevent this from occurring again in the future.\n\nThanks,\n\nSendible Team",
            "nextpage": "1402010570"
        },
        {
            "userimage": "https://graph.facebook.com/588219818/picture",
            "userlink": "https://facebook.com/588219818",
            "link": "https://facebook.com/588219818",
            "created_at_client": "2014-06-06T14:29:44+0000",
            "source": "facebook",
            "sentiment": 0,
            "content": "",
            "id": "588219818_10152471830099819",
            "term": "sendible",
            "favicon": "http://www.google.com/s2/favicons?domain=facebook.com",
            "description": "",
            "username": "Shoshanna J Mashiach",
            "type": "facebooksearch",
            "domain": "facebook.com",
            "title": "They promise they will never do this to U.S.......",
            "nextpage": "1402010570"
        },
        {
            "userimage": "https://graph.facebook.com/574271150/picture",
            "userlink": "https://facebook.com/574271150",
            "link": "https://facebook.com/574271150",
            "created_at_client": "2014-06-06T13:30:59+0000",
            "source": "facebook",
            "sentiment": 0,
            "content": "",
            "id": "574271150_10152484849271151",
            "term": "sendible",
            "favicon": "http://www.google.com/s2/favicons?domain=facebook.com",
            "description": "",
            "username": "Jason J Vautour",
            "type": "facebooksearch",
            "domain": "facebook.com",
            "title": "Jason J Vautour shared a link.",
            "nextpage": "1402010570"
        },
        {
            "userimage": "https://graph.facebook.com/454478881363113/picture",
            "userlink": "https://facebook.com/454478881363113",
            "link": "https://facebook.com/454478881363113",
            "created_at_client": "2014-06-06T11:53:43+0000",
            "source": "facebook",
            "sentiment": 0,
            "content": "",
            "id": "454478881363113_479728652171469",
            "term": "sendible",
            "favicon": "http://www.google.com/s2/favicons?domain=facebook.com",
            "description": "",
            "username": "Kate and Alli Social Marketing",
            "type": "facebooksearch",
            "domain": "facebook.com",
            "title": "Kate and Alli Social Marketing shared a link.",
            "nextpage": "1402010570"
        },
        {
            "userimage": "https://graph.facebook.com/100008309898923/picture",
            "userlink": "https://facebook.com/100008309898923",
            "link": "https://facebook.com/100008309898923",
            "created_at_client": "2014-06-05T23:22:51+0000",
            "source": "facebook",
            "sentiment": 0,
            "content": "",
            "id": "100008309898923_1416218811998435",
            "term": "sendible",
            "favicon": "http://www.google.com/s2/favicons?domain=facebook.com",
            "description": "",
            "username": "Gil Gaines",
            "type": "facebooksearch",
            "domain": "facebook.com",
            "title": "Gil Gaines shared a link.",
            "nextpage": "1402010570"
        }
    ],
    "max_id": 1402010570
}
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```