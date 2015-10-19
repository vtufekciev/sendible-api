To retrieve a user's accounts, make an authenticated GET request.

#### URL: ####
http://sendible.com/api/v2/accounts.json

#### HTTP Methods: ####
GET

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `filter`: Optional. The search string used to filter results by name.
  * `service_type`: Optional. The type of service to search for. E.g. `emailautoresponder`.
  * `include_properties`: Optional. Set this to `true` to have service properties/parameters included in results.
  * `per_page`: Optional.  The number of results to return per page.
  * `page`: Optional. The page number to be returned.

#### Editing an account: ####
To edit an account, you need to open a window with the `connection_url`. After an account is updated, a notification is sent back to the parent window.

#### Success Response: ####
```
{
    "accounts": [
        {
            "sender_type": "bloggerv3",
            "id": 615497,
            "avatar": null,
            "username": "sendibletest",
            "service_image": "http://snd-assets.s3.amazonaws.com/icons/somicro/blogger.png",
            "service_description": "Blogger and Blogspot",
            "connection_url": "/api/v2/connect?service_id=11809&account_id=615497",
            "service_id": 11809,
            "description": "sendibletest"
        },
        {
            "sender_type": "blogspot",
            "id": 605429,
            "avatar": null,
            "username": "sendibleblogger@gmail.com",
            "service_image": "http://snd-assets.s3.amazonaws.com/icons/somicro/blogger.png",
            "service_description": "Blogger and Blogspot",
            "connection_url": "/api/v2/connect?service_id=11809&account_id=605429",
            "service_id": 11809,
            "description": "http://sendibleblogger.blogspot.com"
        },
        {
            "sender_type": "brandmonitor",
            "id": 740644,
            "avatar": null,
            "username": "Sendible Main3 Test",
            "service_image": "https://d3u44nfepqqjcg.cloudfront.net/images/comment-16x16.png",
            "service_description": "Brand and Keyword Monitoring",
            "connection_url": "/api/v2/connect?service_id=53&account_id=740644",
            "service_id": 53,
            "description": "Sendible Main3 Test"
        },
        {
            "sender_type": "brandmonitor",
            "id": 514918,
            "avatar": null,
            "username": "Sendible Test",
            "service_image": "https://d3u44nfepqqjcg.cloudfront.net/images/comment-16x16.png",
            "service_description": "Brand and Keyword Monitoring",
            "connection_url": "/api/v2/connect?service_id=53&account_id=514918",
            "service_id": 53,
            "description": "Sendible Test"
        },
        {
            "sender_type": "brandmonitor",
            "id": 573305,
            "avatar": null,
            "username": "mobisquad",
            "service_image": "https://d3u44nfepqqjcg.cloudfront.net/images/comment-16x16.png",
            "service_description": "Brand and Keyword Monitoring",
            "connection_url": "/api/v2/connect?service_id=53&account_id=573305",
            "service_id": 53,
            "description": "Mobisquad"
        },
        {
            "sender_type": "brandmonitor",
            "id": 573307,
            "avatar": null,
            "username": "entrust bankcard",
            "service_image": "https://d3u44nfepqqjcg.cloudfront.net/images/comment-16x16.png",
            "service_description": "Brand and Keyword Monitoring",
            "connection_url": "/api/v2/connect?service_id=53&account_id=573307",
            "service_id": 53,
            "description": "Entrust Bankcard"
        },
        {
            "sender_type": "brandmonitor",
            "id": 597642,
            "avatar": null,
            "username": "apple",
            "service_image": "https://d3u44nfepqqjcg.cloudfront.net/images/comment-16x16.png",
            "service_description": "Brand and Keyword Monitoring",
            "connection_url": "/api/v2/connect?service_id=53&account_id=597642",
            "service_id": 53,
            "description": "Apple"
        },
        {
            "sender_type": "brandmonitor",
            "id": 597643,
            "avatar": null,
            "username": "android",
            "service_image": "https://d3u44nfepqqjcg.cloudfront.net/images/comment-16x16.png",
            "service_description": "Brand and Keyword Monitoring",
            "connection_url": "/api/v2/connect?service_id=53&account_id=597643",
            "service_id": 53,
            "description": "Android"
        },
        {
            "sender_type": "brandmonitor",
            "id": 728022,
            "avatar": null,
            "username": "london stock exchange",
            "service_image": "https://d3u44nfepqqjcg.cloudfront.net/images/comment-16x16.png",
            "service_description": "Brand and Keyword Monitoring",
            "connection_url": "/api/v2/connect?service_id=53&account_id=728022",
            "service_id": 53,
            "description": "London Stock Exchange"
        },
        {
            "sender_type": "brandmonitor",
            "id": 519402,
            "avatar": null,
            "username": "skin by lovely",
            "service_image": "https://d3u44nfepqqjcg.cloudfront.net/images/comment-16x16.png",
            "service_description": "Brand and Keyword Monitoring",
            "connection_url": "/api/v2/connect?service_id=53&account_id=519402",
            "service_id": 53,
            "description": "Skin by Lovely"
        }
    ]
}
```