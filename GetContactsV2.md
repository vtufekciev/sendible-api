Retrieves a list of the authenticated user's contacts.

#### URL: ####
http://sendible.com/api/v2/contacts.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `filter`: Optional. A JSON string in the following format:
```
{
    "contains": "",
    "owner_id": "1,2", 
    "created_after": "2012-01-01",
    "created_before": "2020-12-21",
    "contact_type", "Lead",
    "custom_fields": [
        {
            "name": "age",
            "operator": "<",
            "value": 12
            

        }
    ]
}
```

Please note:

- owner\_id can consist of a comma separated list of user ID's,

- contact\_type can be `Lead`, `Account` or `Opportunity`.

  * `contact_info` Optional. Only contacts with this contact information is returned. Valid values are: `email`, `sms` or `mixed`.
  * `per_page`: Optional. The number of contacts to return per page. Maximum is 1000.
  * `page`: Optional. The page number to return.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
[
    {
        "image_url": "http://sendible-public.s3.amazonaws.com/images/silhouette.gif",
        "id": 10831941,
        "first_name": "carpas",
        "last_name": "missvalles",
        "full_name": "carpas missvalles",
        "firstName": "carpas",
        "lastName": "missvalles",
        "preference": "Email",
        "email": "aaaa@xxxx.com",
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
    },
    {
        "image_url": "http://sendible-public.s3.amazonaws.com/images/silhouette.gif",
        "id": 10675039,
        "first_name": "Jennifer",
        "last_name": "Coulston",
        "full_name": "Jennifer Coulston",
        "firstName": "Jennifer",
        "lastName": "Coulston",
        "preference": "Email",
        "email": "Jenny@xxxxcom",
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
    },
    {
        "image_url": "http://sendible-public.s3.amazonaws.com/images/silhouette.gif",
        "id": 10586692,
        "first_name": "Panda",
        "last_name": "Ta",
        "full_name": "Panda Ta",
        "firstName": "Panda",
        "lastName": "Ta",
        "preference": "Email",
        "email": "ngan_ta2001@xxxx.com",
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
]
```