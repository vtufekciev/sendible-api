To delete an email template for a given user, make a DELETE call using basic authentication with the template ID.

#### URL: ####
http://sendible.com/api/v2/template.json

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `template_id`: The ID of the template to delete.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{"status": "OK"}
```