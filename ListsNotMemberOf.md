To find all the lists that a service or contact does NOT belong to, make a GET request.

#### URL: ####
http://sendible.com/api/v2/lists_not_member_of.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `item_id`: The `recipient_id` of the service retrieved from the [Services](Services.md) call or the `contact_id` of a contact.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
    {
        "color": "#057b79",
        "list_name": "001_Academy_Newsletter",
        "user_id": 5131,
        "consumers": [],
        "contributors": [],
        "item_count": 10286,
        "id": 35529,
        "list_type": "Mixed"
    }
]
```