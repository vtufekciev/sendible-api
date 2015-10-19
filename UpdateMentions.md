Set sentiment and relevancy for a set of mentions. Make a **GET** call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/mentions

#### HTTP Methods: ####
PUT

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `ids`: list of mention ids separated by commas
  * `sentiment`: Optional. 1 for positive, 0 for neutral, -1 for negative
  * `relevancy`: Optional. 1 for relevant, 0 for irrelevant

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{"result":"Sentiment Updated"}
{"result":"Relevancy Updated"}
{"result":"Sentiment Updated, Relevancy Updated"}
```

#### Error Response: ####
```
{"result":"Error no ID"}
{"result":"Error no Sentiment or Relevancy"}
```