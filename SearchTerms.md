To retrieve a list of previous social searches the authenticated user has made, make a **GET** request using basic authentication.

#### URL: ####
http://sendible.com/api/v2/search_terms

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `per_page`: Optional. The maximum number of results to return. Default is 8.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.


#### Success Response: ####
```
[
    {
        "id": 26576,
        "search_term": "burger king 2"
    },
    {
        "id": 26488,
        "search_term": "hootsuite"
    },
    {
        "id": 26471,
        "search_term": "sendible"
    },
    {
        "id": 25614,
        "search_term": "Sendible Main3 Test"
    },
    {
        "id": 22645,
        "search_term": "jsapi"
    },
    {
        "id": 22571,
        "search_term": "humble bundle"
    },
    {
        "id": 22391,
        "search_term": "studio "
    },
    {
        "id": 22390,
        "search_term": "burger king "
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