To retrieve an avatar for a given email address, make a GETcall without any authentication.

#### URL: ####
http://sendible.com/api/utils/email_avatar.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `email`: The user's email address.
  * `default`: Optional. If no matching avatar is found, this URL will be refurned as default.

#### Authentication: ####
None required.

#### Success Response: ####
```
{"avatar": ""http://www.gravatar.com/avatar/xxxx.png" }
```