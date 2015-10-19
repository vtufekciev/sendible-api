To search for social profiles on Twitter, Facebook, Instagram or LinkedIn make an authenticated GET request.

#### URL: ####
http://sendible.com/api/v2/social_profile_search.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `type`: One of the following: `twitter`, `linkedin`, `facebook`, `instagram`.
  * `q`: The name to search for.
  * `account_id`: Optional. The service id, if available for the authenticated user returned by the [Services](Services.md) API method. Alternatively, just use null.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "profiles": [
        {
            "profile_id": "606240366",
            "profile_name": "Gavin Hammar",
            "bio": "",
            "last_name": "Hammar",
            "profile_picture": "https://graph.facebook.com/606240366/picture",
            "profile_url": "http://facebook.com/606240366",
            "location": "",
            "first_name": "Gavin"
        },
        {
            "profile_id": "587135622",
            "profile_name": "Gavin Hoy",
            "bio": "",
            "last_name": "Hoy",
            "profile_picture": "https://graph.facebook.com/587135622/picture",
            "profile_url": "http://facebook.com/587135622",
            "location": "",
            "first_name": "Gavin"
        },
        {
            "profile_id": "546520281",
            "profile_name": "AudryJo Gavin",
            "bio": "",
            "last_name": "Gavin",
            "profile_picture": "https://graph.facebook.com/546520281/picture",
            "profile_url": "http://facebook.com/546520281",
            "location": "",
            "first_name": "AudryJo"
        }
    ],
    "account_id": 515290
}
```