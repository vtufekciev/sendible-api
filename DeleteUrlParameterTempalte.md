To delete an URL parameter template, make a DELETE call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/url_parameter_template.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `url_parameter_template_id`: The id of the URL parameter template to be deleted.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{"status": "OK"}
```