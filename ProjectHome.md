# Sendible API Documentation #

The Sendible API enables developers to interact with the Sendible web site programmatically via simple HTTP requests.
Sendible exposes its data via a <a href='http://en.wikipedia.org/wiki/Representational_State_Transfer'>REST-based Application Programming Interface (API)</a>. This document is the official reference for that functionality.

To get started, you'll need a Sendible user account and Application ID. Sign up at: http://sendible.com/signup.

Once you've signed up for a Sendible account, you can request an Application ID at: http://sendible.com/developers. You'll need to use the `application_id` in all requests you make to the API.

## Authentication ##
All API endpoints require that authentication credentials be supplied through basic HTTP authentication.

You can authenticate using your Sendible username and password. If you'd prefer not to use your password, you can use your remote API key, which can be found at http://sendible.com/profile/edit.

## REST API ##

### Profile ###
  * <a href='http://code.google.com/p/sendible-api/wiki/Profile'>Retrieve user profile</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/SingleSignOn'>Single sign on</a>
  * <a href='https://snd-store.s3.amazonaws.com/developers/Login%20for%20Developer%20Apps.pdf'>Single sign on (using access key)</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/CreateUserField'>Set custom fields for a user</a>

### Services ###
  * <a href='http://code.google.com/p/sendible-api/wiki/Services'>Retrieve services</a>

### Messages ###
  * <a href='http://code.google.com/p/sendible-api/wiki/GetMessages'>Retrieve messages</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/GetMessage'>Retrieve a message</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/MessageRecipients'>Retrieve message recipients</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/CreateMessage'>Create a message</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/DeleteMessage'>Delete a message</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/UpdateMessage'>Update a message</a>

### Media ###
  * <a href='http://code.google.com/p/sendible-api/wiki/AttachMedia'>Add media to a message</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/DeleteMedia'>Remove media from a message</a>

### Mentions ###
  * <a href='http://code.google.com/p/sendible-api/wiki/GetMentionTerms'>Retrieve mention terms</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/GetMentions'>Retrieve mentions</a>

### Social Inbox ###
  * <a href='http://code.google.com/p/sendible-api/wiki/GetPriorityPosts'>Retrieve priority posts</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/CreatePriorityPostReply'>Reply to a priority post</a>

### Contacts ###
  * <a href='http://code.google.com/p/sendible-api/wiki/GetContacts'>Retrieve contacts</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/GetContact'>Retrieve a contact</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/CreateContact'>Create a contact</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/UpdateContact'>Update a contact</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/DeleteContact'>Delete a contact</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/CreateContactField'>Set a custom field for a contact</a>

### Groups/Lists ###
  * <a href='https://code.google.com/p/sendible-api/wiki/GetLists'>Retrieve all lists belonging to a user</a>
  * <a href='https://code.google.com/p/sendible-api/wiki/GetList'>Retrieve a specific list</a>
  * <a href='https://code.google.com/p/sendible-api/wiki/GetListItems'>Retrieve items within a list</a>
  * <a href='https://code.google.com/p/sendible-api/wiki/AddToList'>Add an item to a list</a>
  * <a href='https://code.google.com/p/sendible-api/wiki/RemoveFromList'>Remove an item from a list</a>
  * <a href='https://code.google.com/p/sendible-api/wiki/CreateList'>Create a new list</a>
  * <a href='https://code.google.com/p/sendible-api/wiki/UpdateList'>Update a list</a>
  * <a href='https://code.google.com/p/sendible-api/wiki/DeleteList'>Delete a list</a>

### Url Shortening ###
  * <a href='http://code.google.com/p/sendible-api/wiki/ShortenUrl'>Shorten a url</a>

### Reports ###
#### Message Reports ####
  * <a href='http://code.google.com/p/sendible-api/wiki/GetMessageReports'>Retrieve message reports</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/GetMessageReport'>Retrieve a message report</a>
#### Account Reports ####
  * <a href='http://code.google.com/p/sendible-api/wiki/GetAccountDetails'>Retrieve account details</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/GetAccountPeriods'>Retrieve valid account reporting periods</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/GetAccountStatistics'>Retrieve account statistics</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/GetAccountPosts'>Retrieve account posts and post responses/comments</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/ExportReport'>Download a full HTML/CSV report</a>

### White Labels ###
  * <a href='http://code.google.com/p/sendible-api/wiki/GetProfiles'>Retrieve user profiles belonging to agency/white label</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/SingleSignOn'>Single sign on</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/CreateWhiteLabelUser'>Create a new user</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/UpdateUser'>Update a user</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/CreateUserField'>Update custom fields for a user</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/GetAccountTypes'>Get Account Types/Plans (for older white label sites)</a>

## Subscribing To Realtime Events ##
Using these API methods, you can configure Sendible to send an update to a URL of your choice when specific events occur for users.
  * <a href='https://code.google.com/p/sendible-api/wiki/CreateAppSubscription'>Create one or more event subscriptions for your application</a>
  * <a href='https://code.google.com/p/sendible-api/wiki/SubscribeUserToEvent'>Subscribe to updates for specific users</a>
  * <a href='http://code.google.com/p/sendible-api/wiki/UnsubscribeUserFromEvent'>Unsubscribe from updates for specific users</a>
  * <a href='https://code.google.com/p/sendible-api/wiki/DeleteAppSubscription'>Delete an event subscription for your application</a>
  * <a href='https://code.google.com/p/sendible-api/wiki/GetAppSubscriptions'>List all event subscriptions for your application.</a>