To retrieve a list of the user's social media mention terms, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/mention-terms.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<keywords>
  <keyword>
   <term_id>238873</term_id>
   <description>Sendible</description>
   <type>mention</type>
   <last_checked_gmt>Thu Mar 22 08:30:27 UTC 2012</last_checked_gmt>
  </keyword>
  <keyword>
   <term_id>312289</term_id>
   <description>Disney</description>
   <type>mention</type>
   <last_checked_gmt>Thu Mar 22 08:14:17 UTC 2012</last_checked_gmt>
  </keyword>
  <keyword>
   <term_id>175851</term_id>
   <description>Mc Donalds</description>
   <type>review</type>
   <last_checked_gmt>Wed Mar 21 12:03:58 UTC 2012</last_checked_gmt>
  </keyword>
</keywords>
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```