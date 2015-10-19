Create a user on a Sendible White Label partner site.

Please note: Before you can create a user, you need to enable automatic billing on your white label. This can be setup in the Admin section under Billing.

#### URL: ####
http://sendible.com/api/v1/user.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
POST

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the user of the white label site.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `white_label_code`: The unique code that identifies your white label site. You can locate this code in the admin section of your white label under details.
  * `account_type_id`: Optional. The ID of the account type that this user will be updated to. To retrieve available account type ID's, please use <a href='http://code.google.com/p/sendible-api/wiki/GetAccountTypes'>this API call</a>.
  * `fullname`: The user's name.
  * `email`: The user's email address.
  * `password`: The user's password.
  * `login`: The users username.
  * `timezone`: Optional. The user's timezone offset from GMT in minutes. Default: The admin user's timezone will be used. In Javascript, this is the value of getTimezoneOffset.
  * `managed_by_id`: Optional. The id of the user managing this user's account (the parent user's id).

#### Success Response: ####
```
<user>
  <email>testing@gmail.com</email>
  <fullname>Test User</fullname>
  <id type="integer">3</id>
  <login>testuser</login>
  <is-pro type="boolean">true</is-pro>
  <account-type-name>Marketer</account-type-name>
  <tokens-remaining type="decimal">347.0</tokens-remaining> 
  <message-credits-remaining type="integer">11585</message-credits-remaining> 
  <api-key>xxxx</api-key> 
  <contact-count type="integer">8105</contact-count> 
  <group-count type="integer">20</group-count> 
  <service-count type="integer">88</service-count> 
</user>
```

#### Error Responses: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```

```
<error>
<type>PaymentFailed</type>
<message>The user could not be updated because the payment failed. </message>
</error>
```

```
<error>
<type>AccessError</type>
<message>Only an admin user belonging to the white label can create a user.</message>
</error>
```

```
<error>
<type>AccountTypeNotFound</type>
<message>Unable to find account type.</message>
</error>
```

```
<error>
<type>InvalidTokenQuantity</type>
<message>No pricing could be found for 10 tokens. Please use a standard bundle quantity.</message>
</error>
```

```
<error>
<type>MissingWhiteLabel</type>
<message>Unable to find white label or automatic billing has not been set up.</message>
</error>
```