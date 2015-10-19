To retrieve a list of the user's social media account details, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/account-details.format

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
<account-details type="array">
   <account-detail>
    <account-name>Resources</account-name>
    <description>Facebook Fan Page</description>
    <id type="integer">198918</id>
    <url>
     http://www.facebook.com/pages/Resources/198906483514676
    </url>
    <avatar>http://graph.facebook.com/198906483514676/picture</avatar>
</account-detail>
<account-detail>
   <account-name>Test Page 3</account-name>
    <description>Facebook Fan Page</description>
    <id type="integer">1150841</id>
    <url>
      http://www.facebook.com/pages/Test-Page-3/158776710828095
    </url>
    <avatar>http://graph.facebook.com/158776710828095/picture</avatar>
   </account-detail>
</account-details>
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```