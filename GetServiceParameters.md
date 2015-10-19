To retrieve parameters for a given service, make an authenticated GET request.

#### URL: ####
http://sendible.com/api/v2/service_parameters.json

#### HTTP Methods: ####
GET

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `service_id`: The id of the service retrieved from this call: [GetServiceGroups](GetServiceGroups.md)

Note: You can understand how see how these parameters are rendered by looking at:
http://sendible.com/services/new/service_id (replace service\_id with the value of the service\_id parameter you're using)

#### Success Response: ####
```
{
    "parameters": [
        {
            "id": 1380,
            "post_description": "This is for your own reference.",
            "parameter_type": "text",
            "parameter_name": "fullname",
            "options": null,
            "category": "config",
            "parameter_description": "Description",
            "isMandatory": true
        },
        {
            "id": 3,
            "post_description": null,
            "parameter_type": "text",
            "parameter_name": "username",
            "options": null,
            "category": "config",
            "parameter_description": "Username or Email",
            "isMandatory": true
        },
        {
            "id": 12,
            "post_description": "This will be automatically populated when you connect your account",
            "parameter_type": "hidden",
            "parameter_name": "session_id",
            "options": null,
            "category": "config",
            "parameter_description": "Session Key"
        },
        {
            "id": 10,
            "post_description": "Select your Facebook page from the list above.",
            "parameter_type": "numeric",
            "parameter_name": "account_id",
            "options": "",
            "category": "config",
            "parameter_description": "Facebook Page",
            "isMandatory": true
        },
        {
            "id": 388,
            "post_description": "If you select yes, links will be extracted from your posts and a link preview with caption and image will be posted below your Facebook update.",
            "parameter_type": "list",
            "parameter_name": "linkPreview",
            "options": "No,Yes",
            "category": "config",
            "parameter_description": "Automatically generate link previews",
            "isMandatory": true
        },
        {
            "id": 1552,
            "post_description": "If you select yes, you can define a link that will appear below each post.",
            "parameter_type": "attribution",
            "parameter_name": "attribution",
            "options": null,
            "category": "config",
            "parameter_description": "Attach an attribution link",
            "isMandatory": true
        },
        {
            "id": 1554,
            "post_description": null,
            "parameter_type": "preview",
            "parameter_name": "preview",
            "options": null,
            "category": "config",
            "parameter_description": "What my posts will look like",
            "isMandatory": true
        },
        {
            "id": 1556,
            "post_description": null,
            "parameter_type": "hidden",
            "parameter_name": "link",
            "options": null,
            "category": "config",
            "parameter_description": "Link",
            "isMandatory": true
        },
        {
            "id": 1558,
            "post_description": null,
            "parameter_type": "hidden",
            "parameter_name": "link_title",
            "options": null,
            "category": "config",
            "parameter_description": "Link Title",
            "isMandatory": true
        },
        {
            "id": 1562,
            "post_description": "Use geotargeting to personalize and segment content to different audiences. To target different fans of the same page, you can add the same fan page service as many times as you like and just change the geotargeting settings.",
            "parameter_type": "targetting",
            "parameter_name": "targetting",
            "options": null,
            "category": "config",
            "parameter_description": "Geotargeting",
            "isMandatory": true
        },
        {
            "id": 21891,
            "post_description": "Set this option to Yes to have full-sized images posts to your page.",
            "parameter_type": "list",
            "parameter_name": "post_image",
            "options": "No,Yes",
            "category": "config",
            "parameter_description": "Post as full-sized image"
        },
        {
            "id": 50,
            "post_description": "This will be automatically populated.",
            "parameter_type": "hidden",
            "parameter_name": "token",
            "options": null,
            "category": "config",
            "parameter_description": "Oauth Token"
        },
        {
            "id": 6499,
            "post_description": null,
            "parameter_type": "hidden",
            "parameter_name": "refresh_token",
            "options": null,
            "category": "config",
            "parameter_description": "Refresh Token"
        },
        {
            "id": 16877,
            "post_description": null,
            "parameter_type": "hidden",
            "parameter_name": "api_key",
            "options": "",
            "category": "config",
            "parameter_description": "Facebook API Key"
        },
        {
            "id": 16878,
            "post_description": null,
            "parameter_type": "hidden",
            "parameter_name": "secret",
            "options": "",
            "category": "config",
            "parameter_description": "Facebook Secret"
        },
        {
            "id": 12994,
            "post_description": "Receive alerts whenever there is new activity on this account.",
            "parameter_type": "list",
            "parameter_name": "notify",
            "options": "Priority Inbox Only,Priority Inbox and Email,Email Only,None",
            "category": "config",
            "parameter_description": "Receive alerts for new activity"
        }
    ],
    "id": 19,
    "category": {
        "is_rich_text": false,
        "category_name": "Social Media Publishing Services"
    },
    "compose_parameters": []
}
```