To send a password reset link to a user, make a GET call without any authentication.

#### URL: ####
http://sendible.com/api/utils/password_reset.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `email`: The user's registered email address. This is where them reset password link will be sent.
  * `redirect_uri`: This is URL-encoded URL that the user will be sent to once they click the reset password link from their email. Please note - an activation link will be appended to this URL when the user receives the email. This will be needed for authenticate the user for password reset. `e.g. http://myapp.com/resetpassword# - this will come through as http://myapp.com/resetpassword#xxxxxxx when included in the reset password email.`

#### Authentication: ####
None required.

#### Success Response: ####
```
{"status": "OK" }
```

#### Error Response: ####
```
{"error": {"type": "NotFound", "message": "We were unable to locate your email address."} }
```