To authenticate against the API and retrieve an access token, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/auth

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `redirect_uri`:  The URI to send the user to after authenticating. Sendible will redirect the user back to this URL with either #error\_type= or #access\_token= appended to the URL. You will need to store the access\_token for any subsequent API requests.
  * `site`: Optional. For white label sites, pass the `site` code when you authenticate.
  * `source`: Optional. Specify `client` or `server` as the source. If `client` is set, the response is sent in the following format:#/success/`access_token` or #/error/`error_message` If `server` is set, the response is sent in the following format: ?error\_type=`errorType`&error\_message=`errorMessage` ?access\_token=`access_token`

#### Authentication: ####
Basic authentication with username and password belonging to the Sendible user.

#### Success Response: ####
```
User is redirected to redirect_uri with #access_token= appended to the URL.
```

#### Error Responses: ####
```
User is redirected to redirect_uri with #error_type= appended to the URL.
```