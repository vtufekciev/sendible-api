To update the wizard status, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/wizard.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `step`: The step of the wizard. Set this to `complete` once the wizard has been processed.
Other options are `step_1`, `step_2`, `complete`.

Include these parameters:

#### If `step` is `step_1` ####
  * `business_name`: The name of the business.
  * `timezone`:  The timezone offset value.
  * `timezone_name`: The name of the timezone.

#### If `step` is `step_2` ####
  * `industry_name`: The name of the industry.
  * `competitors`:  A pipe separated list of competitor names. (e.g. pepsi|coke|sprite)

#### If `step` is `complete` ####
No other parameters are needed.


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{"status": "OK"}
```