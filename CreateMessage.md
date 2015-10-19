To create or schedule a Sendible message for a given user, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/message.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `send_to`: A comma separated list of `recipient_id`'s retrieved using the [Services](Services.md) call, email addresses and/or mobile numbers for SMS.
  * `message_text`: The plain text version of the message.
  * `subject`: Optional. The message subject.
  * `message_rich_text`: Optional. Marked-up version of the message. Accepts HTML.
  * `send_date_client`: Optional. The date and time to send the message. Format: `yyyy-MM-dd HH:mm` e.g. `2012-02-24 23:59:40`
  * `notify_me`: Optional. Whether to send an email notification when the message has been delivered. Accepts `1` or `0`.
  * `status`: Optional. The message status. Accepts "Pending" or "Draft".
  * `timezone_offset_client`: Optional. The number of minutes required to convert the client's time zone to GMT. e.g. `-120`
  * `recurs`: Optional. How frequently this message should be posted. `[xx][H = Hours, D = Days, W = Weeks, M = Months, Y = Years]` e.g. `01H` = Every hour or `05D` = Every 5 days.
  * `recurs_until_client`: Optional. The date at which the recurring message should stop. e.g. `2012-02-24 23:59:40`
  * `tags`: Optional. A comma separated list of tag keywords. Used to categorize blog posts.
  * `media`: Optional. A comma separated list of files or images to attach to the message. Each item in the list must contain the file name with extension and a URL-encoded base64 string representing the data. Format: `file_name_1|base64string_1,file_name_2|base64string_2`. e.g. `logo1w.png|iVBORw0KGgoAAAANSUhEUgAAARMAAABfCAMAAAD8mtMpAAADAFBMVEUAcwsOcRojZitLflOWBR...`
  * `queue_id`: Optional. If the message needs to be added to a SmartQueue include the `queue_id` parameter. Also, set the status to `Queued`


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<msg>
  <status>Pending</status>
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
  <send-date-gmt type="datetime">2012-02-24T10:26:55Z</send-date-gmt>
  <send-date-client type="datetime">2012-02-24T12:26:55Z</send-date-client>
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

#### Error Responses: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```



```
<error>
<type>InsufficientCreditsError</type>
<message>This message requires x Message Credit(s). You've already sent y messages this month and have z Message Credit(s) remaining.</message>
</error>
```



```
<error>
<type>MessageError</type>
<message>Message could not be created.</message>
</error>
```