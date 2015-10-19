To post an action (e.g. like an item), make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v0/post-fetch.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_id`: The account ID for this stream.
  * `handle`: The unique identifier for this stream. This is returned by the [GetStream](GetStream.md) call in the `id` field.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "messages": [
        {
            "comments": [
                {
                    "id": "151591754888713_352403964807490_4027406",
                    "editable": false,
                    "commenter": "London Daily Deals",
                    "commenter_pic": "http://graph.facebook.com/151591754888713/picture",
                    "uid": "151591754888713",
                    "message": "Test",
                    "date": "24 Apr 22:24"
                }
            ],
            "comment_count": 1,
            "editable": false,
            "likes": 0,
            "id": "151591754888713_352403964807490",
            "profile_id": "0",
            "uid": "151591754888713",
            "picture": "http://platform.ak.fbcdn.net/www/app_full_proxy.php?app=26065877776&v=1&size=z&cksum=e17a38410270b4eda01bf266c3fa645c&src=http%3A%2F%2Fstatic-www.kgbdeals.co.uk%2Fdeals%2FGB%2F100411%2F100411_s287x183_3.jpg",
            "link": "http://www.kgbdeals.co.uk/london/deals/101611",
            "account_id": 99579,
            "info": {
                "isRead": 0,
                "id": 520412,
                "isHighlighted": 0
            },
            "link_block": "%3Ctable%20style=%22padding-top:5px;%22%3E%3Ctr%3E%3Ctd%20style=%22border:0;%22%20valign=%22top%22%3E%3Ca%20href=%22http://www.kgbdeals.co.uk/london/deals/101611%22%20target=%22_blank%22%3E%3Cimg%20src=%22http://platform.ak.fbcdn.net/www/app_full_proxy.php?app=26065877776&v=1&size=z&cksum=e17a38410270b4eda01bf266c3fa645c&src=http%253A%252F%252Fstatic-www.kgbdeals.co.uk%252Fdeals%252FGB%252F100411%252F100411_s287x183_3.jpg%22%20style=%22max-width:90px;border:0;%22/%3E%3C/a%3E%3C/td%3E%3Ctd%20style=%22border:0;%22%20valign=%22top%22%3E%3Ctable%20%3E%3Ctr%3E%3Ctd%20style=%22border:0;%22%3E%3Ca%20href=%22http://www.kgbdeals.co.uk/london/deals/101611%22%20target=%22_blank%22%3ETwo%20tickets%20to%20Grand%20Designs%20%E2%80%93%20Grand%20Designs%202012%20%E2%80%93%20London%20-%20kgbdeals%3C/a%3E%3C/td%3E%3C/tr%3E%3Ctr%3E%3Ctd%20style=%22border:0;%22%3E%3Cspan%20class=%22faded%22%3Ewww.kgbdeals.co.uk%3C/span%3E%3C/td%3E%3C/tr%3E%3Ctr%3E%3Ctd%20style=%22border:0;%22%3E%C2%A314%20for%20two%20weekend%20tickets%20to%20Grand%20Designs%20Live%202012%20in%20Docklands%20worth%20up%20to%20%C2%A331.60%20%E2%80%93%20save%20up%20to%2056%25%20for%20a%20wealth%20of%20refit%20tips!%3C/td%3E%3C/tr%3E%3C/table%20%3E%3C/td%3E%3C/tr%3E%3C/table%3E",
            "message": "%3Ca%20href=%22%23%22%20onclick=%22new%20Streams().loadProfile('151591754888713',%2099579,%20'facebook');%20%20%20return%20false;%22%3E%3Cb%3ELondon%20Daily%20Deals%3C/b%3E%3C/a%3E %C2%A314%20for%20two%20weekend%20tickets%20to%20Grand%20Designs%20Live%202012%20in%20Docklands%20worth%20up%20to%20%C2%A331.60%20%E2%80%93%20save%20up%20to%2056%25%20for%20a%20wealth%20of%20refit%20tips!",
            "message_unformatted": "%C2%A314%20for%20two%20weekend%20tickets%20to%20Grand%20Designs%20Live%202012%20in%20Docklands%20worth%20up%20to%20%C2%A331.60%20%E2%80%93%20save%20up%20to%2056%25%20for%20a%20wealth%20of%20refit%20tips!",
            "message_formatted": "%3Ca%20href=%22%23%22%20onclick=%22new%20Streams().loadProfile('151591754888713',%2099579,%20'facebook');%20%20%20return%20false;%22%3E%3Cb%3ELondon%20Daily%20Deals%3C/b%3E%3C/a%3E %C2%A314%20for%20two%20weekend%20tickets%20to%20Grand%20Designs%20Live%202012%20in%20Docklands%20worth%20up%20to%20%C2%A331.60%20%E2%80%93%20save%20up%20to%2056%25%20for%20a%20wealth%20of%20refit%20tips!",
            "screen_name": "London%20Daily%20Deals",
            "subject": "%3Ca%20href=%22%23%22%20onclick=%22new%20Streams().loadProfile('151591754888713',%2099579,%20'facebook');%20%20%20return%20false;%22%3E%3Cb%3ELondon%20Daily%20Deals%3C/b%3E%3C/a%3E %C2%A314%20for%20two%20weekend%20tickets%20to%20Grand%20Designs%20Live%202012%20in%20Docklands%20worth%20up%20to%20%C2%A331.60%20%E2%80%93%20save%20up%20to%2056%25%20for%20a%20wealth%20of%20refit%20tips!",
            "subject_formatted": "%3Ca%20href=%22%23%22%20onclick=%22new%20Streams().loadProfile('151591754888713',%2099579,%20'facebook');%20%20%20return%20false;%22%3E%3Cb%3ELondon%20Daily%20Deals%3C/b%3E%3C/a%3E %C2%A314%20for%20two%20weekend%20tickets%20to%20Grand%20Designs%20Live%202012%20in%20Docklands%20worth%20up%20to%20%C2%A331.60%20%E2%80%93%20save%20up%20to%2056%25%20for%20a%20wealth%20of%20refit%20tips!",
            "subject_unformatted": "%C2%A314%20for%20two%20weekend%20tickets%20to%20Grand%20Designs%20Live%202012%20in%20Docklands%20worth%20up%20to%20%C2%A331.60%20%E2%80%93%20save%20up%20to%2056%25%20for%20a%20wealth%20of%20refit%20tips!",
            "avatar": "https://graph.facebook.com/151591754888713/picture",
            "formattedClientTimeLong": "24 Apr 22:11"
        }
    ],
    "editable": false,
    "type": "facebook"
}
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```