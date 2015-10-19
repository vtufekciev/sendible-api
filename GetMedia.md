To retrieve the list of all media for a given user, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/media.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `user_id`: Optional. The specific user id to retrieve messages for. Use `ALL` to retrieve all media for the team. IF this is not set, then the media for the authenticated user will be returned.
  * `per_page`: Optional. The number of messages to return per page.
  * `page`: Optional. The page number to return.
  * `filter`: Optional. A search string parameter used for filtering results.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "files": [
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
        },
        {
            "id": 3747850,
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
        },
        {
            "id": 3742888,
            "file_name": "c1.png",
            "content_type": "image",
            "file_size": "5099",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "http://files.sendible.com/a/3742888/c1.png",
            "url_med": "http://files.sendible.com/a/3742888/c1.png",
            "url_thumb": "http://files.sendible.com/a/3742888/c1.png"
        },
        {
            "id": 3742883,
            "file_name": "c1.png",
            "content_type": "image",
            "file_size": "5099",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "http://files.sendible.com/a/3742883/c1.png",
            "url_med": "http://files.sendible.com/a/3742883/c1.png",
            "url_thumb": "http://files.sendible.com/a/3742883/c1.png"
        },
        {
            "id": 3742858,
            "file_name": "c1.png",
            "content_type": "image",
            "file_size": "5099",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "http://files.sendible.com/a/3742858/c1.png",
            "url_med": "http://files.sendible.com/a/3742858/c1.png",
            "url_thumb": "http://files.sendible.com/a/3742858/c1.png"
        },
        {
            "id": 3742780,
            "file_name": "c1.png",
            "content_type": "image",
            "file_size": "5099",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "http://files.sendible.com/a/3742780/c1.png",
            "url_med": "http://files.sendible.com/a/3742780/c1.png",
            "url_thumb": "http://files.sendible.com/a/3742780/c1.png"
        },
        {
            "id": 3742715,
            "file_name": "chrysanthemum.jpg",
            "content_type": "image",
            "file_size": "879394",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "http://files.sendible.com/a/3742715/chrysanthemum.jpg",
            "url_med": "http://files.sendible.com/a/3742715/chrysanthemum.jpg",
            "url_thumb": "http://files.sendible.com/a/3742715/chrysanthemum.jpg"
        },
        {
            "id": 3742705,
            "file_name": "desert.jpg",
            "content_type": "image",
            "file_size": "845941",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "http://files.sendible.com/a/3742705/desert.jpg",
            "url_med": "http://files.sendible.com/a/3742705/desert.jpg",
            "url_thumb": "http://files.sendible.com/a/3742705/desert.jpg"
        },
        {
            "id": 3742701,
            "file_name": "chrysanthemum.jpg",
            "content_type": "image",
            "file_size": "879394",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "http://files.sendible.com/a/3742701/chrysanthemum.jpg",
            "url_med": "http://files.sendible.com/a/3742701/chrysanthemum.jpg",
            "url_thumb": "http://files.sendible.com/a/3742701/chrysanthemum.jpg"
        },
        {
            "id": 3742685,
            "file_name": "desert.jpg",
            "content_type": "image",
            "file_size": "845941",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "http://files.sendible.com/a/3742685/desert.jpg",
            "url_med": "http://files.sendible.com/a/3742685/desert.jpg",
            "url_thumb": "http://files.sendible.com/a/3742685/desert.jpg"
        },
        {
            "id": 3742653,
            "file_name": "chrysanthemum.jpg",
            "content_type": "image",
            "file_size": "879394",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "http://files.sendible.com/a/3742653/chrysanthemum.jpg",
            "url_med": "http://files.sendible.com/a/3742653/chrysanthemum.jpg",
            "url_thumb": "http://files.sendible.com/a/3742653/chrysanthemum.jpg"
        },
        {
            "id": 3742607,
            "file_name": "Chrysanthemum.jpg",
            "content_type": "image/jpeg",
            "file_size": "879394",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "https://s3.amazonaws.com/files.sendible.com/3742607/original.jpg",
            "url_med": "https://s3.amazonaws.com/files.sendible.com/3742607/medium.jpg",
            "url_thumb": "https://s3.amazonaws.com/files.sendible.com/3742607/thumb.jpg"
        },
        {
            "id": 3742558,
            "file_name": "Attachment",
            "content_type": "image",
            "file_size": "",
            "link_title": "Announcing%20Sendible's%20Smart%20Queues%20with%20Optimal%20Publishing%20Technology",
            "link_url": "http://bit.ly/XtC89M",
            "link_url_display": "www.youtube.com",
            "link_description": "We%20are%20excited%20to%20announce%20the%20release%20of%20Smart%20Queues:%20A%20clever%20way%20to%20schedule%20content%20for%20publication%20to%20multiple%20social%20media%20channels%20with%20minimum%20effor...",
            "type": "image",
            "url_original": "http://i1.ytimg.com/vi/GkK7xkRWIYw/maxresdefault.jpg?feature=og",
            "url_med": "http://i1.ytimg.com/vi/GkK7xkRWIYw/maxresdefault.jpg?feature=og",
            "url_thumb": "http://i1.ytimg.com/vi/GkK7xkRWIYw/maxresdefault.jpg?feature=og"
        },
        {
            "id": 3742528,
            "file_name": "Koala.jpg",
            "content_type": "image/jpeg",
            "file_size": "780831",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "https://s3.amazonaws.com/files.sendible.com/3742528/original.jpg",
            "url_med": "https://s3.amazonaws.com/files.sendible.com/3742528/medium.jpg",
            "url_thumb": "https://s3.amazonaws.com/files.sendible.com/3742528/thumb.jpg"
        },
        {
            "id": 3742516,
            "file_name": "Attachment",
            "content_type": "image",
            "file_size": "",
            "link_title": "Sport",
            "link_url": "http://bbc.in/xNHIOU",
            "link_url_display": "bbc.co.uk",
            "link_description": "Breaking%20news,%20sport,%20TV,%20radio%20and%20a%20whole%20lot%20more.%20The%20BBC%20informs,%20educates%20and%20entertains%20-%20wherever%20you%20are,%20whatever%20your%20age.",
            "type": "image",
            "url_original": "http://www.bbc.co.uk/bbc.com/promo-content/images/promo_luis_130713.jpg",
            "url_med": "http://www.bbc.co.uk/bbc.com/promo-content/images/promo_luis_130713.jpg",
            "url_thumb": "http://www.bbc.co.uk/bbc.com/promo-content/images/promo_luis_130713.jpg"
        },
        {
            "id": 3742372,
            "file_name": "Attachment",
            "content_type": "image",
            "file_size": "",
            "link_title": "8%20Essential%20Facebook%20Tips%20for%20Businesses%20(Part%201)%20",
            "link_url": "http://bit.ly/166LzLY",
            "link_url_display": "sendible.com",
            "link_description": "You%20probably%20already%20know%20that%20not%20being%20on%20Facebook%20isn%E2%80%99t%20an%20option%20for%20businesses%20anymore.%20If%20you%20don%E2%80%99t,%20take%20my%20word%20for%20it.%20If%20you%20don%E2%80%99t%20want%20to%20take%20my%20word%20for%20it,%20let%20me%20give%20you%20a%20lit",
            "type": "image",
            "url_original": "http://sendible.com/insights/wp-content/uploads/2013/07/Millennials_Sendible-613x400.png",
            "url_med": "http://sendible.com/insights/wp-content/uploads/2013/07/Millennials_Sendible-613x400.png",
            "url_thumb": "http://sendible.com/insights/wp-content/uploads/2013/07/Millennials_Sendible-613x400.png"
        },
        {
            "id": 3742369,
            "file_name": "Attachment",
            "content_type": "image",
            "file_size": "",
            "link_title": "Club%20Notes%2013th%20August%20and%20match%20report%20v%20Tir%20Chonaill%20Gaels",
            "link_url": "http://bit.ly/16I3ybQ",
            "link_url_display": "eireoglondon.org",
            "link_description": "This%20weekend%20we%20play%20St%20Clarets%20in%20the%20league%20out%20in%20Greenford%20at%2012%20noon.%20Training%20continues%20on%20Tuesday%20evening%20in%20Highgate%20Wood%20School,%20N8%208RN%20at%207:30pm,%20for%20more%20information%20please%20contact%20Paul%20...",
            "type": "image",
            "url_original": "http://0.gravatar.com/blavatar/4c0fd74b6b5b246d8ce101d35f6540fe?s=200",
            "url_med": "http://0.gravatar.com/blavatar/4c0fd74b6b5b246d8ce101d35f6540fe?s=200",
            "url_thumb": "http://0.gravatar.com/blavatar/4c0fd74b6b5b246d8ce101d35f6540fe?s=200"
        },
        {
            "id": 3742264,
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
        },
        {
            "id": 3739174,
            "file_name": "How to manage foursquare.png",
            "content_type": "image/png",
            "file_size": "349323",
            "link_title": "",
            "link_url": "",
            "link_url_display": "",
            "link_description": "",
            "type": "image",
            "url_original": "https://s3.amazonaws.com/files.sendible.com/3739174/original.png",
            "url_med": "https://s3.amazonaws.com/files.sendible.com/3739174/medium.png",
            "url_thumb": "https://s3.amazonaws.com/files.sendible.com/3739174/thumb.png"
        },
        {
            "id": 3739167,
            "file_name": "Attachment",
            "content_type": "image",
            "file_size": "",
            "link_title": "Test",
            "link_url": "http://bbc.in/ocgyqw",
            "link_url_display": "bbc.co.uk",
            "link_description": "Breaking%20news,%20sport,%20TV,%20radio%20and%20a%20whole%20lot%20more.%20The%20BBC%20informs,%20educates%20and%20entertains%20-%20wherever%20you%20are,%20whatever%20your%20age.",
            "type": "image",
            "url_original": "http://news.bbcimg.co.uk/media/images/69233000/jpg/_69233209_69233208.jpg",
            "url_med": "http://news.bbcimg.co.uk/media/images/69233000/jpg/_69233209_69233208.jpg",
            "url_thumb": "http://news.bbcimg.co.uk/media/images/69233000/jpg/_69233209_69233208.jpg"
        }
    ],
    "pages": 181
}
```