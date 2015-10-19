To log a new exception, make an authenticated POST request.

#### URL: ####
http://sendible.com/api/v2/error_log.json

#### HTTP Methods: ####
POST

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `message`: The error message.
  * `stacktrace`: A dump of the stack trace and any other useful debug information.
  * `source`: The source of the error. E.g. `web`, `android`, `ios`.
  * `type`: The type of error. E.g. `login`, `contact` etc


#### Success Response: ####
```
{
    "source": "web",
    "message": "test",
    "stacktrace": "test",
    "id": 990860,
    "created_at": "2014/04/06 16:59:59 +0000",
    "user_id": 5131
}
```