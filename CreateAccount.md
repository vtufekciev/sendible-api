To create a new account for a given service, make a POST request to this API endpoint.

#### URL: ####
http://sendible.com/api/v2/account.json

#### HTTP Methods: ####
POST

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `service_id`: The id of the service for which the account is being created.
  * `description`: The name/description of this account. This should usually be the username/description of the account for this service.
  * `parameters`: A JSON object representing the populated parameter names and values for this service. Parameters are retrieved using [GetServiceParameters](GetServiceParameters.md). The format of this JSON object is
```
[
    {
        "parameter_name": "SampleName1",
        "parameter_value": "SampleValue1"
    },
    {
        "parameter_name": "SampleName2",
        "parameter_value": "SampleValue2"
    }

]
```


#### Success Response ####

```
{
    "properties": {
        "token_secret": "VmsbBuS37133PKLOM1INIvAFgkdaXojuYesPNaxRgaqAF",
        "username": "GavinHammar",
        "token": "292943066-s5vEpMSFlt3aZFFhXY5nKrg5FuN5iloGRQvUEhez",
        "notify": "Priority Inbox Only"
    },
    "propertyOverride": "username=GavinHammar,token=292943066-s5vEpMSFlt3aZFFhXY5nKrg5FuN5iloGRQvUEhez,token_secret=VmsbBuS37133PKLOM1INIvAFgkdaXojuYesPNaxRgaqAF,notify=Priority Inbox Only",
    "id": 719216,
    "username": "gavinhammar",
    "sender_type": "twitteroauth",
    "service": {
        "parameters": [
            {
                "post_description": null,
                "id": 3,
                "category": "config",
                "parameter_type": "text",
                "parameter_name": "username",
                "parameter_description": "Username or Email",
                "options": null
            },
            {
                "post_description": "This will be automatically populated.",
                "id": 50,
                "category": "config",
                "parameter_type": "hidden",
                "parameter_name": "token",
                "parameter_description": "Oauth Token",
                "options": null
            },
            {
                "post_description": null,
                "id": 132,
                "category": "config",
                "parameter_type": "hidden",
                "parameter_name": "token_secret",
                "parameter_description": "Oauth Token Secret",
                "options": null
            },
            {
                "post_description": "Receive alerts whenever there is new activity on this account.",
                "id": 12994,
                "category": "config",
                "parameter_type": "list",
                "parameter_name": "notify",
                "parameter_description": "Receive alerts for new activity",
                "options": "Priority Inbox Only,Priority Inbox and Email,Email Only,None"
            }
        ],
        "id": 46,
        "compose_parameters": [],
        "category": {
            "category_name": "Social Media Publishing Services",
            "is_rich_text": false
        }
    }
}
```