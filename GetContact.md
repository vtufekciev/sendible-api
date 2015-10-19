To retrieve the details for a specific contact, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/contact.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `contact_id`: The contact id.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<contact> 
  <addressline1 nil="true"></addressline1> 
  <addressline2 nil="true"></addressline2> 
  <birthday type="date">1990-05-01</birthday> 
  <cellphone nil="true"></cellphone> 
  <city nil="true"></city> 
  <company nil="true"></company> 
  <country nil="true"></country> 
  <email>info@sendible.com</email> 
  <fax nil="true"></fax> 
  <firstName>John</firstName> 
  <id type="integer">3568</id> 
  <lastName>Smith</lastName> 
  <occupation nil="true"></occupation> 
  <sex nil="true"></sex> 
  <state nil="true"></state> 
  <tel nil="true"></tel> 
  <unsubscribed type="integer">0</unsubscribed> 
  <zip nil="true"></zip> 
  <contact-accounts type="array"/> 
</contact> 
```

#### Error Response: ####
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