To update information about the authenticated user's company, make a PUT request.

#### URL: ####
http://sendible.com/api/v2/company.json

#### HTTP Methods: ####
PUT

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.

All parameters are optional:
  * `company_name`: Optional. This is the company name.
  * `company_email`: Optional. This is the company's main email address.
  * `company_website`: Optional.This is the URL to the company's website.
  * `company_favicon`: Optional. This is the URL to the company's website favicon.
  * `company_logo`: Optional. This is the URL to the company logo.
  * `global_url_shortener`: Optional.Set this to the company's default URL shortener. Values include: `bit.ly`, `is.gd`, `goo.gl`, `awe.sm`, `don't shorten`
  * `global_url_shortener_login`: Optional. If supported, you can provide the user's bit.ly username.
  * `global_url_shortener_key`: Optional. If supported, you can provide the user's bit.ly api key.

Optional for white labels:
  * `language`: Optional. The default language code for this white label. E.g. `en` or `es`.
  * `contact_us_url`: Optional. The help URL for this white label site.
  * `ga_tracking_code`: Optional. The Google Analytics tracking code.
  * `html_widget_code`: Optional. The HTML widget code that is appended to the site.
  * `theme`: Optional. The name of the theme to be applied. E.g. {{smoothness}}
  * `custom_css`: Optional. The custom CSS code to be applied to the white label site along with the theme.
  * `menus`: Optional. A JSON object array containing the menu structure. For example:
```
[
        {
            "name": "Google Apps",
            "submenus": [
                {
                    "name": "Calendar",
                    "url": "http://apps.google.com/calendar",
                    "type": "iframe"
                },
                {
                    "name": "Mail",
                    "url": "http://apps.google.com/mail",
                    "type": "url"
                },
                {
                    "name": "Drive",
                    "url": "http://apps.google.com/drive",
                    "type": "iframe"
                }
            ]
        }
]
```

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
"status": "OK"
}

```

#### Error Responses: ####
```
{"error": {"type": "NotFound", "message": "Company could not be found."} }
```

```
{"error": {"type": "PermissionDenied", "message": "Only administrators can update the company information."} }
```