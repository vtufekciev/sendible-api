To retrieve statistics for a user or multi-user subscription, make a GET request.

#### URL: ####
http://sendible.com/api/v2/subscription_info.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `details`: Optional. The details to return. Valid values are `all`, `user_stats`.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "apps": {
        "in_use": 19,
        "total_available": 180
    },
    "billing": {
        "plan": {
            "name": "Premium",
            "is_trial": false,
            "monthly_amount": 699.99,
            "trial_days_remaining": 0
        },
        "users_purchased": 18,
        "discount": {
            "annually": 0.1,
            "quarterly": 0.05,
            "monthly": 0,
            "half_yearly": 0.075
        },
        "amount": 3599.88,
        "card_expiry_year": 2015,
        "card_number": "************1234",
        "card_expiry_month": 5,
        "billing_urls": {
            "add_users": "***********",
            "select_plan": "***********",
            "change_plan": "***********",
            "change_card": "***********"
        },
        "amount_monthly": 299.99,
        "currency": "USD",
        "cycle": 12,
        "next_payment": "2012/12/29 01:45:48 +0000",
       "last_payment": "2012/12/29 01:45:48 +0000",
        "member_since": "2008/08/07 19:39:06 +0000"
    },
    "services": {
        "in_use": 335,
        "total_available": 630000
    },
    "users": {
        "inactive": 2,
        "total_available": 18,
        "active": 17
    }
}
```


#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```