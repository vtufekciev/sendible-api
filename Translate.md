Translate text to the specified language. Returns content as plain text, not in JSON format.

#### URL: ####
http://sendible.com/api/v0/translate

#### HTTP Methods: ####
GET

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `text`: The text to be translated.
  * `lang`: The language code to translate into. E.g. en

#### Success Response: ####
```
This is the text translated.
```

#### Error Response: ####
```
{{
    "error": {
        "type": "InvalidHTTPMethod",
        "message": "PUTisinvalidforthisendpoint."
    }
}
```