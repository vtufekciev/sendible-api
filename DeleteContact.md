To delete a contact, make a DELETE call using basic authentication.

#### URL: ####
http://sendible.com/api/v1/contact.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
DELETE

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `contact_id`: The id of the contact to be deleted.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
<?xml version="1.0" encoding="UTF-8"?>
<result>
  <status>success</status>
</result>
```

#### Error Response: ####
```
<error>
<type>ContactNotFound</type>
<message>Contact could not be found.</message>
</error>
```