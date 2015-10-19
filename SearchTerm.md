To store a search term so that it's added to the list  of previous social searches for the authenticated user, make a **POST** request using basic authentication.

#### URL: ####
http://sendible.com/api/v2/search_term

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `search_term`:. The search term (query) to be stored.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.


#### Success Response: ####
```
    {
        "id": 26576,
        "search_term": "burger king 2"
    }
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```