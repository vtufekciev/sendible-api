To retrieve a list of the user's mentions for a given term, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/mentions.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `term_id`: Optional. The mention term, retrieved using the [GetMentionTerms](GetMentionTerms.md) call. If no `term_id` is provided, mentions for all terms will be returned.
  * `sentiment`: Optional. Retrieve mentions with neutral, positive or negative sentiment. Valid values are `0`, `1` or `-1`.
  * `type`: Optional. The type of mentions to retrieve. Valid values are `blogs`, `microblogs`, `bookmarks`, `comments`, `events`, `images`, `news`, `videos`, `audio`, `questions`, `networks`.
  * `filter`: Optional. Filter mentions by keyword.
  * `per_page`: Optional. The number of mentions to return per page.
  * `page`: Optional. The page number to return.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<mentions type="array">
  <mention>
	<content>
		<a href=\http://shine.yahoo.com/photos/<b><b>DISNEY</b></b>-princesses-were-real-sequel-slideshow/snow-white-photo-2298504-190600838.html\ >http://shine.yahoo.com/photos/<b><b>DISNEY</b></b>-princesses-were-real-sequel-slideshow/snow-white-photo-2298504-190600838.html</a><br/><br/> <a href="http://shine.yahoo.com/photos/<b><b>DISNEY</b></b>-princesses-were-real-sequel-slideshow/snow-white-photo-2298504-190600838.html" target="_blank"><b>If <b>Disney</b> Princesses Were Real: The Sequel</b></a><br/>View the If <b>Disney</b> Princesses Were Real: The Sequel photo gallery on Yahoo! Shine. Find more news related pictures in our photo galleries.<br/><br/> <a href="https://plus.google.com/104739022522671686030/posts/WsDxbQFLW5z" target="_blank"><img src="http://images0-focus-opensocial.googleusercontent.com/gadgets/proxy?container=focus&gadget=a&resize_h=100&url=http%3A%2F%2Fl.yimg.com%2Fbt%2Fapi%2Fres%2F1.2%2F.rrudzwc6_4_NErfcheVrQ--%2FYXBwaWQ9eW5ld3M7Zmk9ZmlsbDtoPTE1MDtxPTg1O3c9MTUw%2Fhttp%3A%2F%2Fmedia.zenfs.com%2Fen-US%2Fblogs%2Fpartner%2F2298504.0.cf.png" /></a>
	</content>
	<created-at-client type="datetime">2012-03-22T10:12:53Z</created-at-client>
	<description>
		<a href=\http://shine.yahoo.com/photos/<b><b>DISNEY</b></b>-princesses-were-real-sequel-slideshow/snow-white-photo-2298504-190600838.html\ >http://shine.yahoo.com/photos/<b><b>DISNEY</b></b>-princesses-were-real-sequel-slideshow/snow-white-photo-2298504-190600838.html</a>
	</description>
	<domain>Google+</domain>
	<favicon>
		http://www.google.com/s2/favicons?domain=plus.google.com
	</favicon>
	<link>
		https://plus.google.com/104739022522671686030/posts/WsDxbQFLW5z
	</link>
	<sentiment type="integer">0</sentiment>
	<source>google+</source>
	<title>
		Reshared post from Marquis Crumpton\n \n\nhttp://shine.yahoo.com/photos/disney-princesses-were-real-...
	</title>
	<userimage>
		https://lh4.googleusercontent.com/-ndWnrdb1jIo/AAAAAAAAAAI/AAAAAAAAAAA/GGnra1PYJIg/photo.jpg?sz=50
	</userimage>
	<userlink>https://plus.google.com/104739022522671686030</userlink>
	<username>Jeremy Zano</username>
	<type>networks</type>
	<term>Disney</term>
  </mention>
  <mention>
	<content/>
	<created-at-client type="datetime">2012-03-22T10:11:31Z</created-at-client>
	<description/>
	<domain>facebook.com</domain>
	<favicon>
		http://www.google.com/s2/favicons?domain=facebook.com
	</favicon>
	<link>
		http://www.facebook.com/100001126359005/posts/325545447502443
	</link>
	<sentiment type="integer">0</sentiment>
	<source>facebook</source>
	<title>
		?? DISNEY EYES LENS??? DPTKAN NEW ARRIVAL LENS HARI INI JUGA... Buy 1-RM38~~~~~FREE POSTAGE Buy 2-RM70~~~~~FREE POSTAGE Buy 3-RM90~~~~~FREE POSTAGE Buy 4-RM130~~~~FREE POSTAGE Buy 5-RM150~~~~FREE POSTAGE --->IF NAK TAMBAH LENS CASE,ADD RM1/PCS
	</title>
	<userimage>http://graph.facebook.com/100001126359005/picture</userimage>
	<userlink>
		http://www.facebook.com/100001126359005/posts/325545447502443
	</userlink>
	<username>Asma Rozi</username>
	<type>networks</type>
	<term>Disney</term>
  </mention>
</mentions>
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```