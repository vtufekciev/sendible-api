To retrieve service groups by category, make an authenticated GET request.

#### URL: ####
http://sendible.com/api/v2/service_groups.json

#### HTTP Methods: ####
GET

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `category_code`: One of the following: `popular`, `social`, `blogs`, `photos`, `bookmarking`, `monitoring`, `apps`.

#### Adding Services: ####
The result set contains an array of services and each service has a `connection_url`. You'll need to open a window redirecting the user to the API host concatenated to the connection url.

For example, using the results below, if a user wants to add a service, you would use:
```
window.open("http://sendible.com/api/v2/connect?service_id=19");
```

You should add an event listener to your page to receive a notification when the services has been added, similar to the following:
```
window.addEventListener("message", receiveMessage, false);

function receiveMessage(event)
	{
	   if (event.origin !== api_url){
	    	return;
		}
		else {
			console.log(event);
		        alert(event.data.status);
		}
	}
```

Once the service has been added, the window will be closed and the parameters will be passed back to your calling page.

#### Success Response: ####
```
{
    "service_groups": [
        {
            "sort_order": 1,
            "name": "Facebook",
            "category_code": "Popular",
            "description": "Facebook",
            "services": [
                {
                    "icon": "http://snd-assets.s3.amazonaws.com/icons/somicro/facebook.png",
                    "title": "Facebook Fan Page",
                    "connection_url": "/api/v2/connect?service_id=19",
                    "description": "Post updates to your Facebook Fan Pages.",
                    "id": 19
                },
                {
                    "icon": "http://snd-assets.s3.amazonaws.com/icons/somicro/twitter.png",
                    "title": "Twitter",
                    "connection_url": "/api/v2/connect?service_id=46",
                    "description": "Post Twitter updates now or in the future.",
                    "id": 46
                }
            ],
            "image_url": null,
            "id": 1
        },
        {
            "sort_order": 2,
            "name": "Twitter",
            "category_code": "Popular",
            "description": "Twitter",
            "services": [],
            "image_url": null,
            "id": 2
        }
    ]
}
```