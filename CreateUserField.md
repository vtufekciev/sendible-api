Allows you to create or update a custom field and set its value for the authenticated user. If the field already exists, it will be updated with the new value, otherwise it will be created.

#### URL: ####
http://sendible.com/api/v1/user_field.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
POST, PUT

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `field_name`: Required. The name of the field you would like to create or update.
  * `field_value`: Required. The value of the `field_name` that you would like to set.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<user>
    <api-key>**************</api-key>
    <email>***@***.com</email>
    <fullname>Sendible</fullname>
    <id type="integer">5131</id>
    <login>sendible</login>
    <is-pro type="boolean">true</is-pro>
    <account-type-name>Premium</account-type-name>
    <total-credits-available type="decimal">12121.0</total-credits-available>
    <tokens-remaining type="decimal">1985.0</tokens-remaining>
    <message-credits-remaining type="integer">126956</message-credits-remaining>
    <contact-count type="integer">10433</contact-count>
    <group-count type="integer">66</group-count>
    <service-count type="integer">208</service-count>
    <contact-fields type="array">
        <contact-field>
            <field-name>location</field-name>
            <field-type>text</field-type>
            <field-value>London</field-value>
        </contact-field>
    </contact-fields>
</user>
```

#### Error Responses: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```