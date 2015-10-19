To update a media file for a given user, make a PUT call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/media.json

#### HTTP Methods: ####
PUT

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `file_id`: The id of the fileto be updated.
  * `file_name`: The new name of the file.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
 {
            "id": 3717139,
            "file_name": "new logo.png",
            "content_type": "image/png",
            "file_size": "5929",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "https://s3.amazonaws.com/files.sendible.com/3717139/original.png",
            "url_med": "https://s3.amazonaws.com/files.sendible.com/3717139/medium.png",
            "url_thumb": "https://s3.amazonaws.com/files.sendible.com/3717139/thumb.png"
        }
```