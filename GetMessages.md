To retrieve a list of the user's Pending/Sent/Draft Sendible messages, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/messages.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `status`: The message status. Possible values are `Pending`, `Draft`,`Sent` or `Queued`.
  * `filter`: Optional. Filter messages by keyword.
  * `per_page`: Optional. The number of messages to return per page.
  * `page`: Optional. The page number to return.
  * `start`: Optional. The date range to return. E.g. `2015-12-19`
  * `end`: Optional. The date range to return. E.g. `2015-12-19`
  * `recipient_ids`: Optional. A comma separated list of recipient ids to filter results by. E.g. {{8211,9892,4432}}}

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<msgs type="array"> 
  <msg> 
    <status>Pending</status> 
    <subject>Test subject</subject> 
    <tags></tags> 
    <user-id type="integer">1</user-id> 
    <recurs>Once</recurs> 
    <recurs-until-gmt type="datetime">2010-07-30T15:51:42Z</recurs-until-gmt> 
    <recurs-until-client type="datetime">2010-07-30T16:51:42Z</recurs-until-client> 
    <message-id type="integer">895</message-id> 
    <message-text>Hello world.</message-text> 
    <message-rich-text>Hello world.</message-rich-text> 
    <notify-me type="integer">0</notify-me> 
    <send-date-gmt type="datetime">2010-07-30T15:51:42Z</send-date-gmt> 
    <send-date-client type="datetime">2010-07-30T16:51:42Z</send-date-client> 
    <send-to>user@gmail.com</send-to> 
    <timezone-offset-client type="integer">-60</timezone-offset-client> 
    <photos type="array"> 
      <photo> 
        <id type="integer">484</id> 
        <name>logo1w.png</name> 
        <file-url>http://sendible.s3.amazonaws.com/_files/484/logo1w.png</file-url> 
      </photo> 
      <photo> 
        <id type="integer">485</id> 
        <name>n1727389556_1512.jpg</name> 
        <file-url>http://sendible.s3.amazonaws.com/_files/485/n1727389556_1512.jpg</file-url> 
      </photo> 
    </photos> 
  </msg> 
  <msg> 
    <status>Pending</status> 
    <subject>Test subject</subject> 
    <tags></tags> 
    <user-id type="integer">1</user-id> 
    <recurs>Once</recurs> 
    <recurs-until-gmt type="datetime">2010-07-30T15:41:35Z</recurs-until-gmt> 
    <recurs-until-client type="datetime">2010-07-30T16:41:35Z</recurs-until-client> 
    <message-id type="integer">894</message-id> 
    <message-text>Hello world.</message-text> 
    <message-rich-text>Hello world.</message-rich-text> 
    <notify-me type="integer">0</notify-me> 
    <send-date-gmt type="datetime">2010-07-30T15:41:35Z</send-date-gmt> 
    <send-date-client type="datetime">2010-07-30T16:41:35Z</send-date-client> 
    <send-to>user@gmail.com</send-to> 
    <timezone-offset-client type="integer">-60</timezone-offset-client> 
    <photos type="array"> 
      <photo> 
        <id type="integer">480</id> 
        <name>logo1w.png</name> 
        <file-url>http://sendible.s3.amazonaws.com/_files/480/logo1w.png</file-url> 
      </photo> 
      <photo> 
        <id type="integer">481</id> 
        <name>n1727389556_1512.jpg</name> 
        <file-url>http://sendible.s3.amazonaws.com/_files/481/n1727389556_1512.jpg</file-url> 
      </photo> 
    </photos> 
  </msg> 
</msgs>
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```