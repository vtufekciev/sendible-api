Retrieve available account types (plans) for a Sendible White Label partner site. (This is for version 1 white label sites.)

Please note: Before you can retrieve available account types, you need to enable automatic billing on your white label. This can be setup in the Admin section under Billing.

#### URL: ####
http://sendible.com/api/v1/account_types.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the administrator of the white label site.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `white_label_code`: The unique code that identifies your white label site. You can locate this code in the admin section of your white label under details.


#### Success Response: ####
```
<account-types type="array">
   <account-type>
      <description>Solo</description>
      <id type="integer">57</id>
      <monthlycostUSD type="decimal">6.99</monthlycostUSD>
      <monthlypriceUSD type="decimal">6.99</monthlypriceUSD>
   </account-type>
   <account-type>
      <description>Pro</description>
      <id type="integer">2</id>
      <monthlycostUSD type="decimal">10.0</monthlycostUSD>
      <monthlypriceUSD type="decimal">10.0</monthlypriceUSD>
   </account-type>
</account-types>
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
<type>AccessError</type>
<message>Only an admin user belonging to the white label can retrieve account types.</message>
</error>
```


```
<error>
<type>MissingWhiteLabel</type>
<message>Unable to find white label or automatic billing has not been set up.</message>
</error>
```