To retrieve receipts for an account make a GET request.

#### URL: ####
http://sendible.com/api/v2/receipts.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "vat_number": "xxxxxxxxxxxxxxxxx",
    "billing_email": "billing@mysite.com,james@mysite.com",
    "billing_user_fullname": "John Smith",
    "billing_user_login": "jsmith01",
    "receipts": [
        {
            "tax": 0,
            "city": "Henderson",
            "zip": "89044",
            "extraInfo": null,
            "created_at": "2013/04/16 16:15:46 +0000",
            "trial": null,
            "card_type": "Visa",
            "card_number": null,
            "amount": 30,
            "street": "2777 Craigmillar st",
            "lastname": "Romano",
            "id": 131974,
            "countrycode": "GB",
            "card_year": "2015",
            "user_id": 5131,
            "firstname": "Rick",
            "description": "Rebranding - Sendible Team",
            "currency": "USD",
            "card_month": "5",
            "status": "Paid",
            "state": "NV",
            "error": null
        },
        {
            "tax": 0,
            "city": "Henderson",
            "zip": "89044",
            "extraInfo": null,
            "created_at": "2013/04/16 16:09:20 +0000",
            "trial": null,
            "card_type": "Visa",
            "card_number": null,
            "amount": 30,
            "street": "2777 Craigmillar st",
            "lastname": "Romano",
            "id": 131973,
            "countrycode": "US",
            "card_year": "2015",
            "user_id": 5131,
            "firstname": "Rick",
            "description": "Rebranding - Sendible Team",
            "currency": "USD",
            "card_month": "5",
            "status": "Paid",
            "state": "NV",
            "error": null
        }
    ]
}
```