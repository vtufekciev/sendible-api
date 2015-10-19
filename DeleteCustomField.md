To delete a custom field, make a DELETE request.

#### URL: ####
http://sendible.com/api/v2/custom_field.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `custom_field_id`: The id of the custom field to delete.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{"status": "OK"}
```


#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```