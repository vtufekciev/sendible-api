To cancel a user's account, make a POST request. If this is an administrator, this will result in the cancellation of all other users in the account.

#### URL: ####
http://sendible.com/api/v2/account_cancellation.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `reason`: Required. The user's reason for cancellation.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
   "status": "OK"
}
```


#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```

```
<error>
<type>PermissionDenied</type>
<message>Only an administrator can delete the account.</message>
</error>
```