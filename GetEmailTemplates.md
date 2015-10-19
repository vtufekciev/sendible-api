To retrieve lists of email templates for a given user, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/templates.json

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
        "template_name": "Deals",
        "user_id": "5131",
        "id": 632
    },
    {
        "template_name": "London Deals",
        "user_id": "5131",
        "id": 624
    }
]
```