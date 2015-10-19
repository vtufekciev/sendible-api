To transfer credits between two users, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/credit_transfer.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `type`: The types of credits to transfer. `sms` OR `email`.
  * `credits`: The number of credits to transfer.
  * `user_id_from`: The `id` of the user to transfer credits from.
  * `user_id_to`: The `id` of the user to transfer credits to.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
"status": "OK"
}
```

#### Error Response: ####
```
{
"error": {
    "type": "InsufficientCredits",
    "message": "The user, john123, does not have enough email credits to transfer.
}
}
    
```