To create a media file for a given user and store it on Sendible, make a POST call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/media.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `media`:  A comma separated list of files or images to attach to the message. Each item in the list must contain the file name with extension and a URL-encoded base64 string representing the data. Format: file\_name\_1|base64string\_1,file\_name\_2|base64string\_2. e.g. logo1w.png|iVBORw0KGgoAAAANSUhEUgAAARMAAABfCAMAAAD8mtMpAAADAFBMVEUAcwsOcRojZitLflOWBR...

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
 {
            "id": 3748430,
            "file_name": "Attachment",
            "content_type": "image",
            "file_size": "",
            "link_title": "",
            "link_url": "http://bbc.in/IUnCfJ",
            "link_url_display": "www.bbc.co.uk",
            "link_description": "Breaking%20news,%20sport,%20TV,%20radio%20and%20a%20whole%20lot%20more.%20The%20BBC%20informs,%20educates%20and%20entertains%20-%20",
            "type": "image",
            "url_original": "http://static.bbci.co.uk/frameworks/barlesque/2.51.1/desktop/3.5/img/blq-blocks_grey_alpha.png",
            "url_med": "http://static.bbci.co.uk/frameworks/barlesque/2.51.1/desktop/3.5/img/blq-blocks_grey_alpha.png",
            "url_thumb": "http://static.bbci.co.uk/frameworks/barlesque/2.51.1/desktop/3.5/img/blq-blocks_grey_alpha.png"
        }
```

#### Error Response: ####
{"error": {"type": "MissingParameter", "message": "Media must contain file name and base64 string separated by a pipe."} }

{"error": {"type": "FileSizeExceeded", "message": "File size must be less than 4MB."} }