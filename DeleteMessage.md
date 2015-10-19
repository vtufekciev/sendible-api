To delete a message, make a DELETE call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/message.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `message_id`: The message's id.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<result>
  <status>success</status>
</result>
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```

OR

```
<error>
<type>MessageNotFoundError</type>
<message>Message could not be found.</message>
</error>
```