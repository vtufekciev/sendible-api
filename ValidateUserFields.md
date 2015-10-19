To retrieve a list of the user's accessible team members/clients, make a GET request.

#### URL: ####
http://sendible.com/api/utils/validate_user_fields.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `field_name`: The name of the field to validate. Values are `username` or `email`.
  * `field_value`: The value of the username or email address to pass to the server.
  * `user_id`: Optional. When updating an existing user, you must pass the user's ID.
  * `format`: Optional. `text` or `json`. If `text` is used, then you will receive a text response.

#### Authentication: ####
Non required.

#### Success Response: ####
If validation is successful:
```
{"status": "OK" }
```


#### Error Response: ####
```
{"error": {"type": "InvalidUsername", "message": "This username is already in use."} }
```

```
{"error": {"type": "InvalidUsername", "message": "Username must be longer than 3 characters."} }
```

```
{"error": {"type": "InvalidEmail", "message": "Email address is invalid."} }
```

```
{"error": {"type": "InvalidUsername", "message": "This username is already in use."} }
```