To retrieve a list of message recipients for a given Sendible message, make a GET call using basic authentication with the user's Sendible username and password

#### URL: ####
http://sendible.com/api/v1/message-recipients.format?type=type

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `message_id`: The message id.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<user-services type="array">
  <user-service>
    <account-name>Twitter - oauth - sendible</account-name>
    <account-type>Twitteroauth</account-type>
    <icon-url>http://www.google.com/s2/favicons?domain=twitter.com</icon-url>
    <recipient-id>6300</recipient-id>
  </user-service>
  <user-service>
    <account-name>Ping.fm - info@sendible.com</account-name>
    <account-type>Pingfm</account-type>
    <icon-url>http://www.google.com/s2/favicons?domain=ping.fm</icon-url>
    <recipient-id>6307</recipient-id>
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
<type>MessageNotFoundError\</type>
<message>Message could not be found.</message>
</error>
```