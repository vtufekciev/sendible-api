To bulk import contacts make a POST request.

#### URL: ####
http://sendible.com/api/v2/import.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `payload`: The raw CSV data.
  * `type`: Set this to `contacts`.
  * `preference`: Set this to `Email`, `SMS` or `Mixed`.
  * `list_id`: Optional. Set this to the list id that these contacts will be added to.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{"rows":2,"status":"Processing","id":34739890}
```