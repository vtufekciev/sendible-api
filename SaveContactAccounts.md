To add contact account information to a contact make a PUT request.

#### URL: ####
http://sendible.com/api/v2/contact_account.json

#### HTTP Methods: ####
PUT

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `contact_id`: The contact id.
  * `type`: The type of the account. This could be one of `facebook`, `twitter`, `linkedin`, `instagram`.
  * `account_id`: The account id used in the [SocialProfileSearch](SocialProfileSearch.md) call.
  * `profile_id`: The profile id returned by [SocialProfileSearch](SocialProfileSearch.md).
  * `profile_url`: The profile url returned by [SocialProfileSearch](SocialProfileSearch.md).
  * `profile_picture`: The profile picture returned by [SocialProfileSearch](SocialProfileSearch.md).
  * `full_name`: The fullname of the contact's account returned by [SocialProfileSearch](SocialProfileSearch.md).
  * `profile_name`: The username of the contact's account returned by [SocialProfileSearch](SocialProfileSearch.md).


#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "id": 3134097,
    "contact_id": 12722250,
    "full_name": "Sendible",
    "profile_id": "15473781",
    "profile_name": "sendible",
    "profile_url": "http://twitter.com/Sendible",
    "profile_picture": "http://pbs.twimg.com/profile_images/3667750807/0d1114cb36f85b8b49e45bacf9bcc485_normal.png",
    "type": "twitter",
    "icon": "http://snd-assets.s3.amazonaws.com/icons/somicro/twitter.png",
    "account_id": 557734
}
```