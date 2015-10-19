To retrieve a list of the user's message reports, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/message-reports.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `filter`: Optional. Filter reports by keyword.
  * `per_page`: Optional. The number of messages to return per page.
  * `page`: Optional. The page number to return.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<message-reports type="array"> 
  <message-report> 
    <clientTime type="datetime">2010-09-13T12:13:57Z</clientTime> 
    <id type="integer">1071280</id> 
    <message-html>Squeak the baby killer whale was moved out of Clacton Pier because of storm damage... what was the year on the Lunchtime Rewind?</message-html> 
    <message-text>Squeak the baby killer whale was moved out of Clacton Pier because of storm damage... what was the year on the Lunchtime Rewind?</message-text> 
    <message-id type="integer">1872924</message-id> 
    <stat-chart>http://chart.apis.google.com/chart?chtt=Message Statistics&amp;chds=0,1&amp;chxl=0:|Comments|Recipients&amp;cht=bvs&amp;chd=t:1,1&amp;chs=350x160&amp;chco=1166BB|377EC6|5D97D1|83AFDC|A9C8E7|CFE0F1&amp;chbh=a&amp;chxt=x&amp;chdl=Comments (1)|Recipients (1)</stat-chart> 
    <subject></subject> 
    <score type="decimal">1.0</score> 
    <messages-photos type="array"/> 
  </message-report> 
  <message-report> 
    <clientTime type="datetime">2010-09-13T10:09:33Z</clientTime> 
    <id type="integer">1071002</id> 
    <message-html>Hi, Joff here with Easy at 11 - a nice way to spend 10mins during a busy Monday! Do you have an 'easy' favourite song? Let me know!</message-html> 
    <message-text>Hi, Joff here with Easy at 11 - a nice way to spend 10mins during a busy Monday! Do you have an 'easy' favourite song? Let me know!</message-text> 
    <message-id type="integer">1872588</message-id> 
    <stat-chart>http://chart.apis.google.com/chart?chtt=Message Statistics&amp;chds=0,3&amp;chxl=0:|Comments|Recipients&amp;cht=bvs&amp;chd=t:3,1&amp;chs=350x160&amp;chco=1166BB|377EC6|5D97D1|83AFDC|A9C8E7|CFE0F1&amp;chbh=a&amp;chxt=x&amp;chdl=Comments (3)|Recipients (1)</stat-chart> 
    <subject></subject> 
    <score type="decimal">3.0</score> 
    <messages-photos type="array"/> 
  </message-report> 
</message-reports>
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```