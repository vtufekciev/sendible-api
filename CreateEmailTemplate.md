To create a new template for the logged in user, make a POST request to this API endpoint.

#### URL: ####
http://sendible.com/api/v2/template.json

#### HTTP Methods: ####
POST

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `template_name`: The name of this template
  * `template_html`: The HTML to represent this template.

#### Success Response ####

```
  {
    "template_name": "Deals",
    "user_id": "5131",
    "template_html": "<!DOCTYPE html PUBLIC \"-//W3C//DTD XHTML 1.0 Transitional//EN\"\n       \"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd\"> \n \n<html xmlns=\"http://www.w3.org/1999/xhtml\" xml:lang=\"en\" lang=\"en\"> \n<head> \n  <meta http-equiv=\"content-type\" content=\"text/html;charset=UTF-8\" /> \n  <link rel=\"alternate\" type=\"application/rss xml\" href=\"/rss.xml\"/>\t\n  <link href=\"http://sendible.com/favicon.gif\" rel=\"icon\" type=\"image/x-png\" /> \n  <link href=\"http://sendible.com/themes/styles.css?1263056931\" media=\"screen\" rel=\"stylesheet\" type=\"text/css\" /> \n  \n  <link href=\"http://sendible.com/themes/default/theme.css?1263081048\" media=\"screen\" rel=\"stylesheet\" type=\"text/css\" /> \n  <title>{Title}</title> \n  \n  <script src=\"http://www.google.com/jsapi\"></script> \n  <script>google.load(\"jquery\", \"1.3\");</script> \n<style>\n.comment_list{\nmargin-top:10px !important;\nfloat:left;\n}\n\n.bodytext img{\nmargin-right:5px;\n}\n</style>\n</head> \n<body> \n \n \n<div id=\"centerbody\"> \n\t<div class=\"sendiblog_header\">{Sendible}</div> \n\t<div class=\"sendiblog_bar\"></div> \n\t<div class=\"header\"><h1><a href=\"{SiteURL}\">{Title}</a></h1></div> \n\t<div class=\"subhead\">{Description}</div> \n\t<div class=\"back_to_blog\">{Back}</div>\n\t<div class=\"sidebar\"> \n\t\t{Views}\n\t\t<p class=\"about\">{About}</p> \n\t\t<div class=\"user_info\"> \n\t\t\t\n\t\t\t<img class=\"profile_border\" alt=\"{OwnerName}\" src=\"{PortraitURL}\" /> \n\t\t\t\n\t\t\t<p class=\"user_title\"><a href=\"#\" onclick=\"$('.user_bio').toggle();return false;\">{OwnerName}'s bio »</a></p> \n\t\t\t<p class=\"user_bio\" style=\"display:none;\">{Profile}</p> \n\t\t</div> \n\t\n\t\t\t\n\t\t<div class=\"sidebarunit\"> \n\t\t\t<form method=\"get\" id=\"searchform\" action=\"{SiteURL}\"> \n\t\t\t<input type=\"hidden\" value=\"\" name=\"sort\"/> \n\t\t\t<input id=\"searchbox\" class=\"search\" type=\"text\" onfocus=\"//$('#searchbox_button').show();\" onblur=\"//$('#searchbox_button').hide();\" onkeyup=\"if (event.keyCode == 13) {$('#searchform').submit();}\" value=\"\" name=\"search\" /> \n\t\t\t<input id=\"searchbox_button\" class=\"searchbox_button\" type=\"submit\" style=\"display: none;\" value=\"Search\"/> \n\t\t\t</form> \n\t\t</div> \n\t\t<div class=\"sidebarunit\"> \n\t\t<div id=\"subscribe_div\"> \n\t\t<a id=\"subscribe_link\" name=\"subscribe_link\" href=\"#\" onclick=\"$('#snd_tbl').toggle();return false;\">Subscribe to the latest deals »</a> \n\t\t\n\t\t</div> \n\t\t</div> \n\t\t<div class=\"sidebarunit\" id=\"newsletter-signup\"> \n\t\t\t<script type=\"text/javascript\" src=\"http://www.sendible.com/widgets/add_contact.js\"></script> \n\t\t\t<script type=\"text/javascript\"> \n\t\t\t\tnewContactForm( {\n\t\t\t\t    api_key:            \"{APIKey}\",\n\t\t\t\t    button_text:        \"Subscribe\",\n\t\t\t\t\tgroup_id:       \t{GroupId},\n\t\t\t\t    show_address:       false,\n\t\t\t\t    show_fax:           false,\n\t\t\t\t    show_occupation:    false,\n\t\t\t\t    show_mobile:        false,\n\t\t\t\t    show_telephone :    false,\n\t\t\t\t    show_company :      false,\n\t\t\t\t    success_url:        \"{SiteURL}?added=true#subscribe_link\",\n\t\t\t\t    failure_url:        \"{SiteURL}?added=true#subscribe_link\"\n\t\t\t\t}\n\t\t\t\t);\n\t\t\t</script> \n\t\t</div> \n\t\t<p> \n\t\t<a style=\"border: medium none ;\" href=\"{SiteURL}/rss.xml\"><img src=\"http://sendible.com/images/rss.png\"/></a> \n\t\t</p> \n\t\t\n\t</div> \n\t\n\t{block:Posts}\t\n\t<div class=\"postunit\"> \n\t\t<div class=\"date\">{PostDay} {PostMonth}, {PostYear}</div> \n\t\t<div class=\"post\"> \n\t\t\t<h2 class=\"posttitle\"><a href=\"{PostURL}\">{PostTitle}</a></h2> \n\t\t\t<div class=\"bodytext\">{Body}</div> \n\t\t\t<div class=\"comment_list\"><p> {Comments}</p></div> \n\t\t</div> \n\t\t<div class=\"comment_list\">{PostedBy}</div> \n\t</div>\n\t{/block:Posts}\n \n\t<div class=\"pagepagination\"> \n\t{Pagination}\n\t</div> \n \n\t\t\n\t</div> \n\t\n\n \n \n</body> \n</html> ",
    "id": 632
}
```