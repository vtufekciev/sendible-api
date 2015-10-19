Allows you to create or update a custom field and set its value for a given contact. If the field already exists, it will be updated with the new value, otherwise it will be created.

#### URL: ####
http://sendible.com/api/v1/contact_field.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `contact_id`: Required. The contact id.
  * `field_name`: Required. The name of the field you would like to create or update.
  * `field_value`: Required. The value of the `field_name` that you would like to set.
**`field_type`: Optional. The type of field that will be created. Valid options are: `text` or `password`.**


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

#### Error Responses: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```

OR

```
<error>
<type>ContactNotFoundError</type>
<message>Contact could not be found.</message>
</error>
```