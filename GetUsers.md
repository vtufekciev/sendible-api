To retrieve a list of the user's accessible team members/clients, make a GET request.

#### URL: ####
http://sendible.com/api/v0/users.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `profile`: Optional. The type of profile to filter users with. Valid values are: `all`, `Team Member`, `Client`, `Administrator`, `Inactive`, `Active` or a comma separated list of permission profile IDs.
  * `filter`: Optional. A search string that can be used to filter results.
  * `advanced_filter`: Optional. A JSON string in the following format:
```
{
    "contains": "",
    "created_after": "2012-01-01",
    "created_before": "2020-12-21",
    "custom_fields": [
        {
            "name": "age",
            "operator": "<",
            "value": 12
            

        }
    ]
}
```
  * `per_page`: Optional. The number of results to return per page. Default is `2000`.
  * `page`: Optional. The page number to return results for.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
If profile is not passed, an array is returned:
```
[
    {
        "lineage": "5131-74797",
        "fullname": "Wally P",
        "api_key": "xxx",
        "login": "wpjr2011"
    },
    {
        "lineage": "59119",
        "fullname": "Ankit Shah",
        "api_key": "xxx",
        "login": "anky"
    }
]
```

Otherwise,
```
{
    "users": [
        {
            "last_login": "2013/09/11 16:14:57 +0000",
            "profile": "Administrator",
            "avatar": "http://www.gravatar.com/avatar/93dd94be007c9fae25f87251f9d6e0e2?s=55&d=http://sendible.com/images/silhouette.png",
            "lineage": "116321",
            "fullname": "john",
            "api_key": "9889daaf681d76fec5d18e804011731540eda0ff",
            "id": 116321,
            "color": "#844451",
            "user_status": "Active (Premium)",
            "parent_user_id": null,
            "is_active": true,
            "login": "johnsendible",
            "email": "xxxxx@xxxx.xxxx"
        },
        {
            "last_login": "2013/09/10 16:33:24 +0000",
            "profile": "Administrator",
            "avatar": "http://www.gravatar.com/avatar/c9dd1ce4aaec3c83ee7a98e99e702c9e?s=55&d=http://sendible.com/images/silhouette.png",
            "lineage": "118082",
            "fullname": "company x",
            "api_key": "59d208c0a5a1fe0cbc919feb82c48bfc2a90da9c",
            "id": 118082,
            "color": "#a593ed",
            "user_status": "Active (Premium)",
            "parent_user_id": null,
            "is_active": true,
            "login": "mesi",
            "email": "xxxxx@xxxx.xxxx"
        },
        {
            "last_login": "2013/09/10 15:37:56 +0000",
            "profile": "Administrator",
            "avatar": "http://www.gravatar.com/avatar/861fa090886f8cd5f16ec6f8d46da57f?s=55&d=http://sendible.com/images/silhouette.png",
            "lineage": "120002",
            "fullname": "Tom Boyd",
            "api_key": "d9387c9821cf21b0894a455903f19d9607f11ca1",
            "id": 120002,
            "color": "#f89eb4",
            "user_status": "Active (Premium)",
            "parent_user_id": null,
            "is_active": true,
            "login": "tomboyd",
            "email": "xxxxx@xxxx.xxxx"
        },
        {
            "last_login": "2013/08/14 17:08:39 +0000",
            "profile": "Administrator",
            "avatar": "http://www.gravatar.com/avatar/1ef7b2156c3700274ad8981140f5a438?s=55&d=http://sendible.com/images/silhouette.png",
            "lineage": "120337",
            "fullname": "xxxx",
            "api_key": "ce69946f14caa718b5bcc794ca3bf114d16198e3",
            "id": 120337,
            "color": null,
            "user_status": "Active (Premium)",
            "parent_user_id": null,
            "is_active": true,
            "login": "xxxxxse",
            "email": "xxxxx@xxxx.xxxx"
        },
        {
            "last_login": "2013/09/12 11:19:29 +0000",
            "profile": "Administrator",
            "avatar": "https://s3.amazonaws.com/files.sendible.com/135875/thumb.png",
            "lineage": "5131",
            "fullname": "Gavin Hammar",
            "api_key": "1e4cde22b70ba03289476bf8fea15f8a641b2ff5",
            "id": 5131,
            "color": "#b6617c",
            "user_status": "Active (Premium)",
            "parent_user_id": null,
            "is_active": true,
            "login": "sendible",
            "email": "xxxxx@xxxx.xxxx"
        }
    ],
    "pageCount": 4,
    "totalResults": 17
}
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```