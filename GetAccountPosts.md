To retrieve daily statistics for a given social media account detail, make a GET call using basic authentication. The days returned represent the date for the given year/month period.

#### URL: ####
http://sendible.com/api/v1/account-posts.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_detail_id`: The account detail id for which to retrieve the valid `yearmonth` codes. Valid `account_detail_id`s can be retrieved using the using the [GetAccountDetails](GetAccountDetails.md) call.
  * `account_statistic_id`: Optional. The `account_statistic_id` for which to retrieve posts. Valid `account_statistic_id`s can be retrieved using the using the [GetAccountStatistics](GetAccountStatistics.md) call.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<posts>
	<post>
		<account-statistic-id type="integer">4006982</account-statistic-id>
		<clientTime type="datetime">2012-03-29T12:55:06Z</clientTime>
		<message-html>hidng plek, body pgal, kpla pyeng ,.,,allahu akbar</message-html>
		<message-text>hidng plek, body pgal, kpla pyeng ,.,,allahu akbar</message-text>
		<metric-1-name>Comments</metric-1-name>
		<metric-1-value type="decimal">0.0</metric-1-value>
		<metric-2-name>Likes</metric-2-name>
		<metric-2-value type="decimal">0.0</metric-2-value>
		<post-link/>
		<post-link-name/>
		<post-picture/>
		<poster-avatar>http://graph.facebook.com/100002382677074/picture</poster-avatar>
		<poster-fullname>BaNnex AZ DeHh</poster-fullname>
		<sentiment type="integer">0</sentiment>
		<post-responses type="array"/>
	</post>
	<post>
		<account-statistic-id type="integer">4006982</account-statistic-id>
		<clientTime type="datetime">2012-03-28T13:45:48Z</clientTime>
		<message-html>
		Sendible I tried to reach your help-desk but I could not. Would you please check why my account ayman@oasisventures.net is suspended? I have a lot of work to do. Thanks
		</message-html>
		<message-text>
		Sendible I tried to reach your help-desk but I could not. Would you please check why my account ayman@oasisventures.net is suspended? I have a lot of work to do. Thanks
		</message-text>
		<metric-1-name>Comments</metric-1-name>
		<metric-1-value type="decimal">1.0</metric-1-value>
		<metric-2-name>Likes</metric-2-name>
		<metric-2-value type="decimal">0.0</metric-2-value>
		<post-link/>
		<post-link-name/>
		<post-picture/>
		<poster-avatar>http://graph.facebook.com/726184005/picture</poster-avatar>
		<poster-fullname>Ayman Albarbary</poster-fullname>
		<sentiment type="integer">0</sentiment>
		<post-responses type="array">
			<post-response>
				<avatar>http://graph.facebook.com/21274802454/picture</avatar>
				<body>
				Could you try sign in now? You should have access again.
				</body>
				<created-at type="datetime">2012-03-28T18:02:39Z</created-at>
				<responder-fullname>Sendible</responder-fullname>
				<responder-identifier>21274802454_10150611646282455_21331651</responder-identifier>
				<sentiment type="integer">0</sentiment>
				<url/>
			</post-response>
		</post-responses>
	</post>
</posts>
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```