To retrieve priority inbox items for a given user, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/priority-posts.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `page`: Optional. The page number to return.
  * `per_page`: Optional. The number of items to return per page. Default is 20.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
    {
        "account_detail": {
            "account_id": 43674,
            "account": {
                "service": {
                    "stream_actions": [
                        {
                            "name": "Like",
                            "action": "like",
                            "can_message": false,
                            "message_prefix": ""
                        },
                        {
                            "name": "Comment",
                            "action": "comment",
                            "can_message": true,
                            "message_prefix": ""
                        }
                    ]
                }
            },
            "account_name": "Sendible",
            "uid": "21274802454"
        },
        "message_type": "Post",
        "responder_fullname": "Rosalia Maria",
        "account_detail_id": 104714,
        "relative_created_at": "8 hours ago",
        "post_link": "",
        "original_message": null,
        "url": null,
        "sentiment": 2,
        "isRead": 0,
        "account_name": "Sendible",
        "post_body": "gostava de fazer 1 pergunta! como é que as notas do jogo sity viil de 11 ou 12 passam para 8? sem que eu tenha comprado seja o que for? é que já não é a 1ª vez que acontece!! e, muito sinceramente começo a ficar cansada !!e, pelo que me tenho percebido há muita gente a deixar este jogo porque por + que as pessoas se esforcem raramente se consegue levar 1 tarefa até ao fim pois é impossivel! a não ser que as pessoas não façam + nada o que não me parece! boa noite e obrigada.",
        "uid": "100000103828925",
        "id": 28428019,
        "responder_identifier": "100000103828925",
        "responder_avatar": "http://graph.facebook.com/100000103828925/picture",
        "message_html": "",
        "account_avatar": "http://graph.facebook.com/21274802454/picture",
        "post_picture": "",
        "message_text": "",
        "service_name": "facebook(page)",
        "service_image": "https://d3u44nfepqqjcg.cloudfront.net/images/icons/facebook_page.gif",
        "created_at": "2012/05/18 00:20:11 +0000"
    }
]
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```