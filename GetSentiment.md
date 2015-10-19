To retrieve the sentiment for a mention term.
Make a **GET** call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/sentiment

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_id`: One or more mention terms ID, retrieved using the [GetMentionTerms](GetMentionTerms.md) call. Can have more than one mention by separating the mentions by commas.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
{
	"type" : "microblogs",
	"content" : "",
	"sentiment" : 0,
	"created_at_client" : "2014/05/28 06:22:27 +0000",
	"domain" : "twitter.com",
	"source" : "twitter",
	"username" : "JRMA421",
	"userimage" : "http:\/\/pbs.twimg.com\/profile_images\/471514458184245248\/JTgQH4v3_normal.jpeg",
	"link" : "http:\/\/twitter.com\/JRMA421\/statuses\/471521861973852161",
	"description" : "",
	"id" : 200028632,
	"term" : "burger king",
	"title" : "RT @ckuldys22: burger king is closed life is over",
	"userlink" : "http:\/\/twitter.com\/JRMA421",
	"favicon" : "http:\/\/www.google.com\/s2\/favicons?domain=twitter.com"
}, 
{
	"type" : "microblogs",
	"content" : "",
	"sentiment" : 0,
	"created_at_client" : "2014/05/28 06:22:20 +0000",
	"domain" : "twitter.com",
	"source" : "twitter",
	"username" : "andykuzuki",
	"userimage" : "http:\/\/pbs.twimg.com\/profile_images\/466074362102030336\/7ccUgUjU_normal.jpeg",
	"link" : "http:\/\/twitter.com\/andykuzuki\/statuses\/471521834866065408",
	"description" : "",
	"id" : 200028633,
	"term" : "burger king",
	"title" : "@denkimouse In Argentina Burger King has a special menu for the world cup, with little round french fries (noisette potatoes?), it's cute.",
	"userlink" : "http:\/\/twitter.com\/andykuzuki",
	"favicon" : "http:\/\/www.google.com\/s2\/favicons?domain=twitter.com"
}, 
{
	"type" : "microblogs",
	"content" : "",
	"sentiment" : 0,
	"created_at_client" : "2014/05/28 06:21:58 +0000",
	"domain" : "twitter.com",
	"source" : "twitter",
	"username" : "VincentWYedlin",
	"userimage" : "http:\/\/pbs.twimg.com\/profile_images\/434462845707628544\/-KkyCUzb_normal.jpeg",
	"link" : "http:\/\/twitter.com\/VincentWYedlin\/statuses\/471521740775256064",
	"description" : "",
	"id" : 200028634,
	"term" : "burger king",
	"title" : "\u201c@DebbyRyan: bring a friend; wear a crown.\u201d \u2014You might be too young, but do you remember when you could get a crown at Burger King? ",
	"userlink" : "http:\/\/twitter.com\/VincentWYedlin",
	"favicon" : "http:\/\/www.google.com\/s2\/favicons?domain=twitter.com"
}, 
{
	"type" : "microblogs",
	"content" : "",
	"sentiment" : 0,
	"created_at_client" : "2014/05/28 06:21:31 +0000",
	"domain" : "twitter.com",
	"source" : "twitter",
	"username" : "nisichaa",
	"userimage" : "http:\/\/pbs.twimg.com\/profile_images\/451991688685162497\/Of5yjNDD_normal.jpeg",
	"link" : "http:\/\/twitter.com\/nisichaa\/statuses\/471521630494003200",
	"description" : "",
	"id" : 200028635,
	"term" : "burger king",
	"title" : "Buang receh",
	"userlink" : "http:\/\/twitter.com\/nisichaa",
	"favicon" : "http:\/\/www.google.com\/s2\/favicons?domain=twitter.com"
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