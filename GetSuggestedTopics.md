The topic search endpoint is a read-only resource used for searching a specific topic. It could also be used to generate an auto-completing field for searching such topics. This endpoint returns a JSON array of topics that match the search query.

#### URL: ####
http://sendible.com/api/v2/suggested_topics.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `query`: A part of the query to search for topics for. E.g. `social med`

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
  "topics": [
    "Social Media", 
    "Social Media Marketing", 
    "Social Media Management", 
    "Social Media Strategy", 
    "Social Media Optimization", 
    "Social Media Measurement", 
    "Corporate Social Media"
  ]
}
```