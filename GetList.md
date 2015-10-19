To retrieve an existing list, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/list.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `list_id`: The id of the list to retrieve.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "consumers": [],
    "contributors": [],
    "id": 630,
    "user_id": 5131,
    "list_type": "Social",
    "list_name": "Sendible Twitter"
}
```