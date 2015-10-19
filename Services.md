Retrieve the list of social media services, groups and contacts belonging to the authenticated user.

#### URL: ####
http://sendible.com/api/v1/services.format?type=type

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `type`: Possible values are `all`, `social`, `email`, `sms`, `group`, `contacts`
  * `filter`: Optional. Filter services and/or recipients by keyword.
  * `per_page`: Optional. Number of results to return per page. Default: `100`
  * `page`: Optional. The page number to return. Default: `1`

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<user-services type="array">
  <user-service>
    <account-name>Facebook note - SendibleWeb</account-name>
    <account-type>Facebook(note)</account-type>
    <icon-url>http://sendible.com/images/facebook.png</icon-url>
    <recipient-id>6304</recipient-id>
    <total-pages type="integer">4</total-pages>
  </user-service>
  <user-service>
    <account-name>Facebook page - Amazon</account-name>
    <account-type>Facebook(page)</account-type>
    <icon-url>http://sendible.com/images/facebook.png</icon-url>
    <recipient-id>6296</recipient-id>
    <total-pages type="integer">4</total-pages>
  </user-service>
  <user-service>
    <account-name>Facebook page - Sendible</account-name>
    <account-type>Facebook(page)</account-type>
    <icon-url>http://sendible.com/images/facebook.png</icon-url>
    <recipient-id>6289</recipient-id>
    <total-pages type="integer">4</total-pages>
  </user-service>
</user-services>
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```

OR

```
<error>
<type>ServicesNotFound</type>
<message>No services could be found.</message>
</error>
```