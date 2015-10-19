To create a new URL parameter template for the logged in user, make a POST request to this API endpoint.

#### URL: ####
http://sendible.com/api/v2/url_parameter_template.json

#### HTTP Methods: ####
POST

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `preset_name`: The name of this URL parameter template
  * `querystring`: The querystring that will be appended to URLs that are shortened when using this template.
  * `always_use`: Set this to `1` or `0`.

#### Success Response ####

```
    {
        "user_id": 5131,
        "always_use": 0,
        "querystring": "utm_source=test",
        "preset_name": "Custom GA",
        "cannot_delete": 0,
        "id": 2
    }
```