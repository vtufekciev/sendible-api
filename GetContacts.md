Retrieves a list of the authenticated user's contacts.

#### URL: ####
http://sendible.com/api/v1/contacts.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `filter`: Optional. Filter contacts by keyword.
  * `field_name`: Optional. Find contacts that have had this specific field name set using <a href='http://code.google.com/p/sendible-api/wiki/CreateContactField'>this method</a>.
  * `field_value`: Optional. Find contacts that have had this specific field value set using <a href='http://code.google.com/p/sendible-api/wiki/CreateContactField'>this method</a>.
  * `per_page`: Optional. The number of contacts to return per page. Maximum is 1000.
  * `page`: Optional. The page number to return.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<contacts type="array"> 
  <contact> 
    <addressline1></addressline1> 
    <addressline2></addressline2> 
    <birthday type="date" nil="true"></birthday> 
    <cellphone></cellphone> 
    <city></city> 
    <company></company> 
    <country></country> 
    <email>tom@smith.com</email> 
    <fax></fax> 
    <firstName>Tom</firstName> 
    <id type="integer">3566</id> 
    <lastName>Smith</lastName> 
    <occupation></occupation> 
    <sex></sex> 
    <state></state> 
    <tel></tel> 
    <unsubscribed type="integer">1</unsubscribed> 
    <zip></zip> 
    <contact-accounts type="array"> 
      <contact-account> 
        <accountTypeName>Facebook Wall Post</accountTypeName> 
        <account-id>121212111</account-id> 
        <id type="integer">6304</id> 
        <username>sendibleweb</username> 
      </contact-account> 
    </contact-accounts>
    <contact-fields>
      <contact-field> 
        <field-name>password</field-name> 
        <field-value>1234</field-value> 
      </contact-field> 
    </contact-fields>
  </contact> 
</contacts> 
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```