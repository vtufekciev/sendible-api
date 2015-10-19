Get Feeds or Previous Searches for Twitter/Facebook Search.
Make a **GET** call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/storyFeeds
#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `feed_type`: Set this to **feed** to get feeds or set this to **search** to get previous searches for Twitter/Facebook Search
  * `search`: Optional. To filter this search
  * `total`: Optional. Results to retrieve

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
{
	"feed_url" : "surface pro",
	"user_id" : 99583,
	"id" : 26407,
	"feed_type" : "search",
	"feed_name" : "surface pro",
	"created_at" : "2014/05/23 15:23:57 +0000"
},
{
	"feed_url" : "hello",
	"user_id" : 99583,
	"id" : 26404,
	"feed_type" : "search",
	"feed_name" : "hello",
	"created_at" : "2014/05/23 13:38:37 +0000"
},
{
	"feed_url" : "#1DWelcomeToBrazil",
	"user_id" : 99583,
	"id" : 26109,
	"feed_type" : "search",
	"feed_name" : "#1DWelcomeToBrazil",
	"created_at" : "2014/05/07 14:01:02 +0000"
}
]
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```