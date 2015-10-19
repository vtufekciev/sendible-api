To check if a URL is a white label, make an unauthenticated GET request.

#### URL: ####
http://sendible.com/api/utils/site_lookup.json

#### HTTP Methods: ####
GET

#### Authentication: ####
None.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `url`: The URL of the current site.

#### Success Response: ####
```
{
    "stylesheet_url": "http://login.tavsy.com/styling?site_name=Tavsy&type=webapp",
    "api_endpoint": "http://login.tavsy.com",
    "site_code": "Tavsy",
    "is_wl": true,
    "site_name": "Tavsy",
    "favicon_url": "https://snd-store.s3.amazonaws.com/0/Tavsy/Tavsy_16x16.png",
    "logo_url": "https://snd-store.s3.amazonaws.com/0/Tavsy/Tavsy_110x40.png"
}
```

OR

{
> "is\_wl": false
}

#### Error Response: ####
{
> "error": {
> > "type": "NotFound",
> > "message": "This site has not yet been configured. "

> }
}