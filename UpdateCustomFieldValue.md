To update values for custom fields make a PUT call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/custom_fields.json

#### HTTP Methods: ####
PUT

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `category`: The category of fields to retrieve. Valid values are `user`, `contact` or `account`.
  * `identifier`: The ID of the entity to update. This represents `user_id`, `contact_id` or `account_id`.
  * `field_values`: A comma separated list of key value pairs separated by equals. The values should be URL encoded. i.e. `field1=value1,field2=value2,field3=value3` Example: `twitter_handle=aplusk,blog_url=http%3A%2F%2Fmyblog.com`


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
"status": "OK"
```

#### Error Responses: ####
```
{"error": {"type": "MissingParameter", "message": "The category parameter is missing."} }
```

```
{"error": {"type": "MissingParameter", "message": "The identifier parameter is missing."} }
```