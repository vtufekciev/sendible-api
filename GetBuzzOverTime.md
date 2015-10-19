To retrieve a list of the mentions for each day in the last two weeks for a one or more mentions. Includes a breakdown of negative and positive sentiment. To get neutral sentiment subtract negative and positive sentiment from the total. Make a **GET** call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/buzzOverTime

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_id`: One or more mention terms ID, retrieved using the GetMentionTerms call. Can have more than one mention by separating the mentions by commas.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
"result" : [
	{
		"negative" : "18",
		"created_date_str" : "28 May",
		"created_date" : "2014-05-28",
		"positive" : "24",
		"total" : "136"
	},
	{
		"negative" : "26",
		"created_date_str" : "27 May",
		"created_date" : "2014-05-27",
		"positive" : "61",
		"total" : "407"
	},
	{
		"negative" : "14",
		"created_date_str" : "26 May",
		"created_date" : "2014-05-26",
		"positive" : "57",
		"total" : "339"
	},
	{
		"negative" : "31",
		"created_date_str" : "25 May",
		"created_date" : "2014-05-25",
		"positive" : "58",
		"total" : "307"
	},
	{
		"negative" : "30",
		"created_date_str" : "24 May",
		"created_date" : "2014-05-24",
		"positive" : "43",
		"total" : "262"
	},
	{
		"negative" : "20",
		"created_date_str" : "23 May",
		"created_date" : "2014-05-23",
		"positive" : "55",
		"total" : "354"
	},
	{
		"negative" : "39",
		"created_date_str" : "22 May",
		"created_date" : "2014-05-22",
		"positive" : "97",
		"total" : "452"
	},
	{
		"negative" : "34",
		"created_date_str" : "21 May",
		"created_date" : "2014-05-21",
		"positive" : "88",
		"total" : "458"
	},
	{
		"negative" : "16",
		"created_date_str" : "20 May",
		"created_date" : "2014-05-20",
		"positive" : "119",
		"total" : "404"
	},
	{
		"negative" : "51",
		"created_date_str" : "19 May",
		"created_date" : "2014-05-19",
		"positive" : "53",
		"total" : "413"
	},
	{
		"negative" : "17",
		"created_date_str" : "18 May",
		"created_date" : "2014-05-18",
		"positive" : "54",
		"total" : "315"
	},
	{
		"negative" : "22",
		"created_date_str" : "17 May",
		"created_date" : "2014-05-17",
		"positive" : "61",
		"total" : "350"
	},
	{
		"negative" : "20",
		"created_date_str" : "16 May",
		"created_date" : "2014-05-16",
		"positive" : "71",
		"total" : "375"
	},
	{
		"negative" : "70",
		"created_date_str" : "15 May",
		"created_date" : "2014-05-15",
		"positive" : "106",
		"total" : "768"
	}
]
}
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```