Log the user in to their Sendible account and direct to the default page or a page you specify.

#### URL: ####
http://sendible.com/api/v1/single-sign-on

#### HTTP Methods: ####
GET

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `redirect_to`: Optional. The URL to direct users to after signing in. If you leave this out, the user will be redirected to the Sendible or White Label homepage.

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```