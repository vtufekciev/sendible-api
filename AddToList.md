To add an item to a list, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/list_add.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `list_id`: The id of the list to add this item to.
  * `item_id`: The `recipient_id` of the service retrieved from the [Services](Services.md) call or the `contact_id` of a contact.



#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
   "status": "OK"
}
```