To move an item from one list to another, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/list_move.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `list_from_id`: The id of the list to move this item from.
  * `list_to_id`: The id of the list to move this item into.
  * `item_id`: The id of the service to be moved.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
   "status": "OK"
}
```