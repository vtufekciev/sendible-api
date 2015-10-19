To retrieve suggested content for a user or by topic, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/suggested_content.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `topics`: Optional. One or more topics, separated with OR.
  * `from`: Optional. The record number to start from. Useful for paging. 50 results are returned at a time.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "items": {
        "results": [
            {
                "site_name": "ESPN.com",
                "shares": 30799,
                "body": "Cavs' Shumpert drops hip-hop track called 'The Offs'",
                "title": "Cavs' Shumpert drops hip-hop track called 'The Offs'",
                "site_image": "https://s3.amazonaws.com/espn.com.png",
                "keywords": "NBA, Iman Shumpert, Cleveland Cavaliers,NBA, Iman Shumpert, Cleveland Cavaliers",
                "published": 1429757973,
                "images": {
                    "thumbnail": {
                        "size": [
                            100,
                            100
                        ],
                        "url": "http://a4.espncdn.com/combiner/i?img=%2Fphoto%2F2015%2F0410%2Fnba_g_irving%2Dshumpert_mb_1296x1296.jpg"
                    }
                },
                "site_twitter_handle": "espn",
                "index": 0,
                "site_domain": "espn.com",
                "source": "espn.com",
                "url": "http://espn.go.com/espn/story/_/page/instantawesome-imanshumpert-150422/cleveland-cavaliers-iman-shumpert-drops-hip-hop-track-offs-2015-nba-playoffs",
                "share_url": "http://espn.go.com/espn/story/_/page/instantawesome-imanshumpert-150422/cleveland-cavaliers-iman-shumpert-drops-hip-hop-track-offs-2015-nba-playoffs"
            }
}
```