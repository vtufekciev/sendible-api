To reply to a priority post, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/priority-post-reply.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `priority_post_id`: The ID of the priority post that you are responding to, retrieved using the [GetPriorityPosts](GetPriorityPosts.md) call.
  * `message`: The message text to respond with.


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<msg>
    <status>Pending</status>
    <subject />
    <tags />
    <user-id type="integer">52231</user-id>
    <recurs />
    <recurs-until-gmt type="datetime">2012-04-03T12:52:52Z</recurs-until-gmt>
    <recurs-until-client type="datetime">2012-04-03T13:52:52Z</recurs-until-client>
    <message-id type="integer">8882304</message-id>
    <message-text>@MattAster Yes, we do. Take a look at this post: http://goo.gl/XJgwf</message-text>
    <message-rich-text>@MattAster Yes, we do. Take a look at this post: http://goo.gl/XJgwf</message-rich-text>
    <notify-me type="integer">0</notify-me>
    <send-date-gmt type="datetime">2012-04-03T11:52:52Z</send-date-gmt>
    <send-date-client type="datetime">2012-04-03T12:52:52Z</send-date-client>
    <send-to>P1451603</send-to>
    <timezone-offset-client type="integer">-60</timezone-offset-client>
    <photos type="array" />
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
<type>UnableToSaveError</type>
<message>>This post reply could not be created.</message>
</error>
```

```
<error>
<type>PostNotFoundError</type>
<message>>This post could not be found.</message>
</error>
```