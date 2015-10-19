Retrieves the details about a specific Sendible message.

#### URL: ####
http://sendible.com/api/v1/message.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `message_id`: The message's id.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<msg>
  <status>Sent</status>
  <subject></subject>
  <tags nil="true"></tags>
  <user-id type="integer">1</user-id>
  <recurs>Once</recurs>
  <recurs-until-gmt type="datetime">2009-11-12T10:26:55Z</recurs-until-gmt>
  <recurs-until-client type="datetime">2009-11-12T12:26:55Z</recurs-until-client>
  <message-id type="integer">5</message-id>
  <message-text>test to FF.</message-text>
  <message-rich-text>&lt;!DOCTYPE html PUBLIC &quot;-//W3C//DTD XHTML 1.0 Transitional//EN&quot; &quot;http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd&q
uot;&gt;
&lt;html&gt;
&lt;head&gt;
&lt;title&gt;&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
&lt;p&gt;test to FF.&lt;/p&gt;
&lt;/body&gt;
&lt;/html&gt;</message-rich-text>
  <notify-me type="integer">0</notify-me>
  <send-date-gmt type="datetime">2009-11-12T10:26:55Z</send-date-gmt>
  <send-date-client type="datetime">2009-11-12T12:26:55Z</send-date-client>
  <send-to>&quot;Friendfeed - hamgav&quot; &lt;5453&gt;</send-to>
  <timezone-offset-client type="integer">-120</timezone-offset-client>
  <photos type="array"> 
    <photo> 
      <id type="integer">484</id> 
      <name>logo1w.png</name> 
      <file_url>http://sendible.s3.amazonaws.com/_files/484/logo1w.png</file_url> 
    </photo> 
    <photo> 
      <id type="integer">485</id> 
      <name>n1727389556_1512.jpg</name> 
      <file_url>http://sendible.s3.amazonaws.com/_files/485/n1727389556_1512.jpg</file_url> 
    </photo> 
  </photos> 
</msg>
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
<type>MessageNotFoundError</type>
<message>Message could not be found.</message>
</error>
```