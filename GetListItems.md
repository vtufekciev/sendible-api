To retrieve all items in a list, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/list_items.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `list_id`: The id of the list whose items you want to retrieve.
  * `per_page`: Optional. The number of results to return per page.
  * `page`: Optional. The page number for the results you wish to retrieve. Default: 1.
  * `filter`: Optional. The keyword/string to filter results by.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
    {
        "id": 2711061,
        "account": {
            "service": {
                "title": "Twitter",
                "icon": "http://twitter.com/phoenix/favicon.ico"
            },
            "description": "sendible"
        }
    },
    {
        "id": 2724824,
        "account": {
            "service": {
                "title": "Twitter",
                "icon": "http://twitter.com/phoenix/favicon.ico"
            },
            "description": "VishalPindoriya"
        }
    }
]
```

OR, if the list type is Email or SMS:


```
[
    {
        "id": 10180451,
        "user_id": null,
        "title": "Achoeng Adhie",
        "icon": "http://sendible-public.s3.amazonaws.com/images/silhouette.gif",
        "item_type": "Email",
        "description": "xxxxx@xxxxx.com"
    },
    {
        "id": 10180452,
        "user_id": null,
        "title": "Islam Samy",
        "icon": "http://sendible-public.s3.amazonaws.com/images/silhouette.gif",
        "item_type": "Email",
        "description": "xxxxx@xxxxx.com"
    }
]
```