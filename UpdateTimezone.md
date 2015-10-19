To update a user's timezone, make an authenticated PUT request.

#### URL: ####
http://sendible.com/api/v2/timezone.json

#### HTTP Methods: ####
PUT

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `timezone_name`: The name of the timezone.
  * `timezone`: The timezoneOffsetClient value from the browser.
  * `update_messages`: Optional. Set this to 1 to apply the timezone update to messages too. (Default is 0).
  * `autotimezone`: Optional. Set this to 0 if the user should not be prompted to change their timezone again. (Default is 1)


#### Success Response: ####
```
{
"status": "OK"
}
```