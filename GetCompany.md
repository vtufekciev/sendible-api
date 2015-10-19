To retrieve information about the authenticated user's company, make a GET request.

#### URL: ####
http://sendible.com/api/v2/company.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "total_team_members": 14,
    "company_favicon": "http://www.google.com/s2/favicons?domain=sendible.com",
    "company_name": "Sendible Test",
    "account_owner": "James Kane",
    "team_members": [
        {
            "fullname": "Peter Smith",
            "avatar": "http://www.gravatar.com/avatar/193b886f0da67a7935e42e108f2ad433?s=55&d=http://sendible.com/images/silhouette.png"
        },
        {
            "fullname": "Jon Smith",
            "avatar": "http://www.gravatar.com/avatar/db2d1a58da10b9b99c9c98ae518b8054?s=55&d=http://sendible.com/images/silhouette.png"
        }
    ],
    "company_website": "http://xxxxxxx.com",
    "company_email": "xxxxxx",
    "company_logo": "http://ccc.com/xxxxxx.jpg"
}
```

If this is a white label company, you'll receive the following additional fields:

```
{
    "theme": "smoothness",
    "language": "es",
    "contact_us_url": "http://support.mysite.com",
    "ga_tracking_code": "UA-47698035-1",
    "html_widget_code": "<div>Hello world</div>",
    "custom_css": ".body {color: red;} div {color: green;}",
    "menus": [
        {
            "name": "Google Apps",
            "submenus": [
                {
                    "name": "Calendar",
                    "url": "http://apps.google.com/calendar",
                    "type": "iframe"
                },
                {
                    "name": "Mail",
                    "url": "http://apps.google.com/mail",
                    "type": "url"
                },
                {
                    "name": "Drive",
                    "url": "http://apps.google.com/drive",
                    "type": "iframe"
                }
            ]
        }
    ]
}
```