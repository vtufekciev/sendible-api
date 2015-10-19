Update an existing user on a Sendible White Label partner site.

Please note: Before you can update a user, you need to enable automatic billing on your white label. This can be setup in the Admin section under Billing.

#### URL: ####
http://sendible.com/api/v1/user.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
PUT

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the user of the white label site.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `white_label_code`: The unique code that identifies your white label site. You can locate this code in the admin section of your white label under details.
  * `account_type_id`: Optional. The ID of the account type that this user will be updated to. To retrieve available account type ID's, please use <a href='http://code.google.com/p/sendible-api/wiki/GetAccountTypes'>this API call</a>.
  * `tokens`: Optional. The number of tokens to add to this user. The value can be `500`, `1000`, `5000` or `10000`.
  * `disable`: Optional. Set this to `true` to disable this user account. When set to `false`, include the parameter `user_api_key` to represent the user's `api_key` that needs to be re-enabled.



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