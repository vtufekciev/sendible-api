To retrieve an account, make an authenticated GET request.

#### URL: ####
http://sendible.com/api/v2/account.json

#### HTTP Methods: ####
GET

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_id`: The ID belonging to the account.

#### Editing an account: ####
To edit an account, you need to open a window with the `connection_url`. After an account is updated, a notification is sent back to the parent window.

#### Success Response: ####
```
{
    "properties": {
        "message": "Thanks for opting in.",
        "mapresponse": "none",
        "number": "+442033223363",
        "group_id": "36395",
        "smskeyword": "sendible"
    },
    "id": 603003,
    "propertyOverride": "smskeyword=sendible,number=+442033223363,group_id=36395,mapresponse=none,message=Thanks for opting in.",
    "service": {
        "parameters": [
            {
                "parameter_description": "Opt-In  keyword",
                "parameter_type": "keyword",
                "id": 3477,
                "category": "config",
                "parameter_name": "smskeyword",
                "options": null,
                "post_description": "This is the keyword that contacts need to include in their text messages to opt in."
            },
            {
                "parameter_description": "Pick a number",
                "parameter_type": "valuelist",
                "id": 8761,
                "category": "config",
                "parameter_name": "number",
                "options": "|Available inbound numbers...,|United States (+1),+14423337363|&nbsp;&nbsp;-&nbsp;&nbsp;(442) 333-SEND,+19177467283|&nbsp;&nbsp;-&nbsp;&nbsp;(917) 7-GOSAVE,+17179678278|&nbsp;&nbsp;-&nbsp;&nbsp;(717) 96-START,+13158202559|&nbsp;&nbsp;-&nbsp;&nbsp;(315) 820-2559,|United Kingdom (+44),+442033223363|&nbsp;&nbsp;-&nbsp;&nbsp;(203) 32-ADDME,+442033224636|&nbsp;&nbsp;-&nbsp;&nbsp;(203) 322-INFO",
                "post_description": "Select an opt-in number from the list and share this with your customers. <br/>Want your own number? Contact us about getting a <a href=\"mailto:$email?subject=Custom Number\">custom number/shortcode</a> for your company."
            },
            {
                "parameter_description": "Add contacts to this group",
                "parameter_type": "group",
                "id": 3479,
                "category": "config",
                "parameter_name": "group_id",
                "options": null,
                "post_description": "Add contacts who have opted in via SMS to this group."
            },
            {
                "parameter_description": "Map response to",
                "parameter_type": "contact_field",
                "id": 8731,
                "category": "config",
                "parameter_name": "mapresponse",
                "options": null,
                "post_description": "The mobile number will be captured automatically but you can define which contact field should store the response."
            },
            {
                "parameter_description": "Automatic response",
                "parameter_type": "message_maxlength",
                "id": 3481,
                "category": "config",
                "parameter_name": "message",
                "options": "160",
                "post_description": "Enter a message that will be sent out to new contacts."
            }
        ],
        "compose_parameters": [],
        "id": 2319,
        "reply_via_filter": null,
        "category": {
            "is_rich_text": false,
            "category_name": "Email and SMS Services"
        },
        "stream_actions": []
    },
    "username": "sendible",
    "sender_type": "smsgroup"
}
```