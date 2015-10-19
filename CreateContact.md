To create a new contact, make a POST call using basic authentication. The new contact will be added to the address book of the authenticated user.

#### URL: ####
http://sendible.com/api/v1/contact.format

#### Formats: ####
Replace `format` with either `xml` or `json`

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `first_name`: The contact's first name.
  * `last_name`: The contact's last name.
  * `owner_id`: Optional. The Sendible user ID that owns this contact.
  * `email`: Optional. The contact's email address.
  * `cellphone`: Optional.The contact's mobile number.
  * `birthday`: Optional. The contact's date of birth. Format: `yyyy-MM-dd` e.g. `2012-02-24`
  * `sex`: Optional. The contact's gender. Accepts `male` or `female`.
  * `city`: Optional. The contact's city.
  * `country`: Optional. The contact's country.
  * `zip`: Optional. The contact's zip/postcode.
  * `state`: Optional. The contact's state.
  * `occupation`: Optional. The contact's occupation.
  * `addressline1`: Optional. The first line of the contact's address.
  * `addressline2`: Optional. The second line of the contact's address.
  * `fax`: Optional. The contact's fax number.
  * `company`: Optional. The contact's company.
  * `tel`: Optional. The contact's telephone number.
  * `image_url`: Optional. The contact's avatar/profile URL.
  * `notes`: Optional. Notes about this contact.
  * `preference`: Optional. `Email` or `SMS`.
  * `bio`: Optional. The contact's bio information.
  * `website_url`: Optional. The contact's website URL.
  * `list_ids`: Optional. A comma separated mailing list ID's that this contact will be added to.
  * `contact_type`: Optional. Either `Lead`, `Account` or `Opportunity`.
  * `lead_source`: Optional. One of the following:
```
Google AdWords
Google (organic)
Other Search Engines
Social Media
Automation
Cold Calling/Telemarketing
Advertising
Custom Referral
Word of Mouth (Non Customers)
Expo/Seminar
Direct Mail
Email Marketing
Unknown
```

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
  {
        "image_url": "",
        "id": 10831941,
        "notes": "",
        "first_name": "carpas",
        "last_name": "missvalles",
        "full_name": "carpas missvalles",
        "firstName": "carpas",
        "lastName": "missvalles",
        "preference": "Email",
        "email": "xxxx@xxx.com",
        "company": "",
        "occupation": "",
        "birthday": "",
        "cellphone": "",
        "tel": "",
        "fax": "",
        "sex": "",
        "city": "",
        "addressline1": "",
        "addressline2": "",
        "country": "",
        "state": "",
        "zip": "",
        "unsubscribed": 0,
        "accounts": []
    }
    
```