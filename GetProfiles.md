Retrieves all the user profiles belonging to the authenticated user. If the authenticated is a white label or agency administrator, then all users belonging to the white label/agency will be returned.

#### URL: ####
http://sendible.com/api/v1/profiles.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.

#### Success Response: ####
```
<users type="array"> 
  <user> 
    <api-key>xxxx</api-key> 
    <email>user@sendible.com</email> 
    <fullname>Admin</fullname> 
    <id type="integer">1</id> 
    <login>username</login> 
    <is-pro type="boolean">true</is-pro> 
    <account-type-name>Marketer</account-type-name> 
    <total-credits-available type="decimal">2222.0</total-credits-available> 
    <api_key>ABCD1234</api_key> 
  </user> 
</users> 
```

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```