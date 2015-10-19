To update an existing user, make a PUT call using basic authentication.

#### URL: ####
http://sendible.com/api/v2/user.json

#### HTTP Methods: ####
PUT

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `user_id`: The ID of the user to update.
  * `user_api_key`: The API key of the user to update.
  * `fullname`: The name of the user.
  * `email`: The email address of the user.
  * `login`: The username of the user.
  * `password`: Optional. The password of the user.
  * `profile`: Either `administrator`, `team member` or `client`.
  * `manager_of`: Optional. A comma separated list of user IDs that this user can manage.

Additional optional parameters:
  * `managed_by_id`: Optional. The user ID of the user that manages this user. Default: None.
  * `approval_from_ids`: Optional. A comma-separated list of user ID's that need to approve this user's content before it is published.
  * `permission_profile_id`: Optional. The permission profile ID to set for the user.
  * `timezone`: Optional. The user's timezone offset from GMT in minutes. Default: The admin user's timezone will be used. In Javascript, this is the value of `getTimezoneOffset`.
  * `language`: Optional. The user's default language, as an ISO 639-1 code. For example, English would be set as `en`.
  * `clock_format`: Optional. The user's preferred clock format, i.e. a 12 hour clock or a 24 hour clock. Values can be `12` or `24`.
  * `marketing`: Optional. Set this to `1` if the user can receive marketing updates from Sendible. Alternatively, set it to `0`.
  * `url_shortener`: Optional. Set this to the user's default URL shortener. Values include: `bit.ly`, `is.gd`, `goo.gl`, `awe.sm`, `don't shorten`
  * `url_shortener_login`: Optional. If supported, you can provide the user's bit.ly username.
  * `url_shortener_key`: Optional. If supported, you can provide the user's bit.ly api key.
  * `image_shortener`: Optional. Provide the image shortener for posting images to Twitter. Values include: `Twitter`, `Twitpic`,`Yfrog`
  * `preference`: Optional. Set the user's publishing preference. This includes whether to always display the rich text editor or not. Values are `default`, `rte_on`, `rte_off`.
  * `is_paused`: Optional. Set this to `1` to pause this user's publishing, or `0` to unpause the user's posts.
  * `security_question`: Optional. Set the user's security question. This is used when a user signs from an unrecognized location.
  * `security_answer`: Optional. Set the user's security answer. This is used when a user signs from an unrecognized location.
  * `valid_ips`: Optional. A commas separated list of valid IP addresses. A user will be prompted to enter security question and answer details if signing in from a non-listed IP.
  * `session_days`: Optional. The number of days before the user's access\_token expires.
  * `photo_id`: Optional. The ID of the photo returned from the [UploadMedia](UploadMedia.md) call.
  * `desktop_notifications`: Optional. Set to 1 if enabled, or 0 if disabled.
  * `remove_url`: Optional. Set to 1 if enabled, or 0 if disabled.
  * `color`: Optional. Set this to a hex color. E.g. `#ffffff`
  * `bitly_pro_domain`: Optional. Set this to the bit.ly pro domain.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "profile": "Team Member",
    "lineage": "122068",
    "is_active": true,
    "fullname": "Test User",
    "api_key": "c48c7db283e1d1b57f1449d1c02d6083b0e1e6a2",
    "last_login": "2013/09/25 13:59:13 +0000",
    "id": 122068,
    "color": "#000000",
    "avatar": "http://www.gravatar.com/avatar/4b13c1a4f17c731280e51faead7bc1f3?s=55&d=http://sendible.com/images/silhouette.png",
    "user_status": "Active (Premium)",
    "parent_user_id": null,
    "login": "xpxaaaaaa",
    "email": "infobbbaaa123@sendible.com",
    "bitly_pro_domain": "snd.bl"
}
```

#### Error Responses: ####
```
{"error": {"type": "MissingParameter", "message": "The profile parameter is missing."} }
```

```
{"error": {"type": "InvalidUsername", "message": "This username is already in use."} }
```

```
{"error": {"type": "InvalidUsername", "message": "This email is already in use."} }
```

```
{"error": {"type": "InvalidUsername", "message": "Username must be longer than 3 characters."} }
```