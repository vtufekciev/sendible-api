To shorten a given url, make a GET call using basic authentication. Where available, Sendible will use the authenticated user's link shortening preferences.

#### URL: ####
http://sendible.com/api/v1/shorten.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `url`: The long url to shorten.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<result>
 <status>success</status>
 <url>http://is.gd/dWSYh</url>
</result>
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```