Retrieve the details for a given `report_id` by making a GET request using basic authentication.

#### URL: ####
http://sendible.com/api/v1/message-report.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `report_id`: The message report id. Retrieved using the <a href='http://code.google.com/p/sendible-api/wiki/GetMessageReports'>message reports</a> call.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<message-report>
  <clientTime type="datetime">2010-09-12T15:59:11Z</clientTime>
  <message-html>
&lt;html&gt;
&lt;head&gt;
&lt;title&gt;&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
&lt;p&gt;Burnout is sneaky&amp;mdash;it doesn't happen overnight&amp;mdash;but t
he stages have classic signs. Clueing in to them can help you sidestep a workout
 slump: http://bit.ly/cXrFix&lt;/p&gt;
&lt;/body&gt;
&lt;/html&gt;</message-html>
  <message-text>Burnout is sneaky&#8212;it doesn't happen overnight&#8212;but th
e stages have classic signs. Clueing in to them can help you sidestep a workout
slump: http://bit.ly/cXrFix</message-text>
  <report-id type="integer">1069562</report-id>
  <subject></subject>
  <score type="decimal">1834.0</score>
  <messages-photos type="array">
    <messages-photo>
      <photo-id type="integer">47908</photo-id>
      <file-name>4 Stages of Exercise Burnout &#8212; And How to Avoid Them</fil
e-name>
      <file-url>http://www.active.com/Assets/Fitness/WH14287.jpg</file-url>
      <file-type>image</file-type>
    </messages-photo>
  </messages-photos>
  <message-recipients type="array">
    <message-recipient>
      <accountName>Facebook page - C25K Fan Page</accountName>
      <recipient-first-name>Status</recipient-first-name>
      <recipient-identifier>311542</recipient-identifier>
      <recipient-last-name>Update</recipient-last-name>
      <icon>/images/facebook_page.gif</icon>
    </message-recipient>
  </message-recipients>
  <message-statistics type="array">
    <message-statistic>
      <code>Click</code>
      <stat-value type="integer">1822</stat-value>
    </message-statistic>
    <message-statistic>
      <code>Comment</code>
      <stat-value type="integer">12</stat-value>
    </message-statistic>
  </message-statistics>
 <responses type="array">
    <response>
      <avatar>http://profile.ak.fbcdn.net/profile-ak-snc1/v22944/426/25/q1000004
89381805_5137.jpg</avatar>
      <body>I'm in Cape Coral have been going to a local gym off and on it is ha
rd to get motivated sometimes but I do try to get there at least two or three ti
mes a week when I do go. It would be easier if there was someone like a gym budd
y that also needed motivating to go to the gym. But I will check out the website
.</body>
      <created-at type="datetime">2010-09-13T05:12:01Z</created-at>
      <responder-fullname>Debbie Fisher Riddling</responder-fullname>
      <responder-identifier>100000489381805</responder-identifier>
      <response-type>Comment</response-type>
      <service-name>Facebook(page)</service-name>
    </response>
    <response>
      <avatar>http://profile.ak.fbcdn.net/hprofile-ak-snc4/hs462.snc4/48821_6057
02829_5037_q.jpg</avatar>
      <body>The best way to find races is to visit active.com.  You can put in t
he dates and event type you want and then narrow the search with your zip code.
 It's basically the best thing ever!</body>
      <created-at type="datetime">2010-09-12T19:59:05Z</created-at>
      <responder-fullname>Audrey Hill</responder-fullname>
      <responder-identifier>605702829</responder-identifier>
      <response-type>Comment</response-type>
      <service-description>Facebook Fan Page</service-description> 
    </response>
 </responses>
</message-report>
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
<type>ParametersMissing</type>
<message>The required parameters for this method are: report_id.</message>
</error>
```

OR

```
<error>
<type>ReportNotFoundError</type>
<message>Report could not be found.</message>
</error>
```