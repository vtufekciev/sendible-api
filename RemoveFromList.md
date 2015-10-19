To remove an item to a list, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/list_remove.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `list_id`: The id of the list to remove this item from.
  * `item_id`: The id of the service or contact to be removed.


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
   "status": "OK"
}
```