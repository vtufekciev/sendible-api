To retrieve details about a particular user's profile from a stream, make a GET call using basic authentication.

#### URL: ####
http://sendible.com/api/v0/profile.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_id`: The account ID for this stream.
  * `handle`: The user's profile identifier. This is returned by the [GetStream](GetStream.md) call in the `uid` field.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "username": "George%20Smith",
    "fullname": "George%20Smith",
    "picture": "http://graph.facebook.com/815407909/picture?type=normal",
    "location": "Location:%20N/A",
    "joined": "",
    "url": "http://www.facebook.com/profile.php?id=815407909",
    "details": "%3Ctable%20style=%22width:100%25;%20line-height:20px;%22%3E%3Ctr%3E%3Ctd%20style=%22width:95px;vertical-align:top;%22%3E%3Cimg%20src=%22http://graph.facebook.com/815407909/picture?type=normal%22%20style=%22width:85px;border:1px%20solid%20gainsboro;padding:2px;%22/%3E%3C/td%3E%3Ctd%20style=%22vertical-align:top;%22%3E%3Cspan%20style=%22font-weight:bold;%20font-size:%20180%25;%22%3EDennis%20Hammar%3C/span%3E%3Cbr/%3E%3Ca%20style=%22font-weight:bold;%20font-size:%20110%25;%22%20href=%22http://www.facebook.com/profile.php?id=815407909%22%20target=%22_blank%22%3Ehttp://www.facebook.com/profile.php?id=815407909%3C/a%3E%3Cbr/%3ELocation:%20N/A%3Cbr/%3E%3Cspan%20style=%22color:%20%23777;font:%20italic%20normal%20normal%2014px/18px%20Georgia,%20serif;%22%3E%3C/span%3E%3Cdiv%20style=%22margin-top:10px;%22%3E%3C/div%3E%3Cdiv%20style=%22margin-top:10px;%22%3E%3Cb%3ERecent%20photos%20of%20Dennis%20Hammar:%3C/b%3E%3Cbr/%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://sphotos.xx.fbcdn.net/hphotos-ash3/535173_10150772747211054_710016053_11299405_1186118767_n.jpg%5C'%20height=%5C'453%5C'%20width=%5C'604%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=10150772747211054&set=p.10150772747211054&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-c.ak.fbcdn.net/hphotos-ak-ash3/535173_10150772747211054_710016053_11299405_1186118767_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://sphotos.xx.fbcdn.net/hphotos-ash4/207253_10150162355077910_815407909_6624884_3146570_n.jpg%5C'%20height=%5C'540%5C'%20width=%5C'720%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=10150162355077910&set=p.10150162355077910&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-a.ak.fbcdn.net/hphotos-ak-ash4/207253_10150162355077910_815407909_6624884_3146570_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://a7.sphotos.ak.fbcdn.net/hphotos-ak-snc6/163942_486887737909_815407909_5784621_8023165_n.jpg%5C'%20height=%5C'540%5C'%20width=%5C'720%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=486887737909&set=a.163424107909.118917.815407909&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-g.ak.fbcdn.net/hphotos-ak-snc6/163942_486887737909_815407909_5784621_8023165_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://a2.sphotos.ak.fbcdn.net/hphotos-ak-ash2/17840_255701302909_815407909_3238796_1180954_n.jpg%5C'%20height=%5C'453%5C'%20width=%5C'604%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=255701302909&set=a.11623722909.18690.815407909&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-b.ak.fbcdn.net/hphotos-ak-ash2/17840_255701302909_815407909_3238796_1180954_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://a7.sphotos.ak.fbcdn.net/hphotos-ak-snc6/9935_163424112909_815407909_2681832_8028291_n.jpg%5C'%20height=%5C'582%5C'%20width=%5C'604%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=163424112909&set=a.163424107909.118917.815407909&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-g.ak.fbcdn.net/hphotos-ak-snc6/9935_163424112909_815407909_2681832_8028291_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://sphotos.xx.fbcdn.net/hphotos-ash4/291_67655915600_607395600_3404047_2337_n.jpg%5C'%20height=%5C'604%5C'%20width=%5C'402%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=67655915600&set=a.67655455600.129779.607395600&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-c.ak.fbcdn.net/hphotos-ak-ash4/291_67655915600_607395600_3404047_2337_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://a4.sphotos.ak.fbcdn.net/hphotos-ak-snc7/291_67655970600_607395600_3404057_5624_n.jpg%5C'%20height=%5C'604%5C'%20width=%5C'403%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=67655970600&set=a.67655455600.129779.607395600&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-d.ak.fbcdn.net/hphotos-ak-snc7/291_67655970600_607395600_3404057_5624_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://sphotos.xx.fbcdn.net/hphotos-ash4/291_67453080600_607395600_3396973_2666_n.jpg%5C'%20height=%5C'402%5C'%20width=%5C'604%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=67453080600&set=a.67452385600.129507.607395600&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-f.ak.fbcdn.net/hphotos-ak-ash4/291_67453080600_607395600_3396973_2666_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://sphotos.xx.fbcdn.net/hphotos-snc7/257_54315735600_607395600_2974822_1123_n.jpg%5C'%20height=%5C'453%5C'%20width=%5C'604%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=54315735600&set=a.54314510600.115165.607395600&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-b.ak.fbcdn.net/hphotos-ak-snc7/257_54315735600_607395600_2974822_1123_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://sphotos.xx.fbcdn.net/hphotos-ash4/239_12142472909_815407909_430659_3780_n.jpg%5C'%20height=%5C'455%5C'%20width=%5C'604%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=12142472909&set=a.11395817909.18499.815407909&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-d.ak.fbcdn.net/hphotos-ak-ash4/239_12142472909_815407909_430659_3780_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://a3.sphotos.ak.fbcdn.net/hphotos-ak-ash4/239_12142482909_815407909_430661_4386_n.jpg%5C'%20height=%5C'603%5C'%20width=%5C'461%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=12142482909&set=a.11395817909.18499.815407909&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-c.ak.fbcdn.net/hphotos-ak-ash4/239_12142482909_815407909_430661_4386_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://sphotos.xx.fbcdn.net/hphotos-snc7/239_12142477909_815407909_430660_4078_n.jpg%5C'%20height=%5C'603%5C'%20width=%5C'469%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=12142477909&set=a.11395817909.18499.815407909&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-e.ak.fbcdn.net/hphotos-ak-snc7/239_12142477909_815407909_430660_4078_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://a8.sphotos.ak.fbcdn.net/hphotos-ak-ash4/239_11691912909_815407909_421820_6515_n.jpg%5C'%20height=%5C'453%5C'%20width=%5C'604%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=11691912909&set=a.11623722909.18690.815407909&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-h.ak.fbcdn.net/hphotos-ak-ash4/239_11691912909_815407909_421820_6515_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://a2.sphotos.ak.fbcdn.net/hphotos-ak-ash4/239_11691312909_815407909_421771_3837_n.jpg%5C'%20height=%5C'604%5C'%20width=%5C'453%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=11691312909&set=a.11623722909.18690.815407909&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-b.ak.fbcdn.net/hphotos-ak-ash4/239_11691312909_815407909_421771_3837_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3Cdiv%20style=%22float:left;%22%3E%3Cdiv%20onclick=%22jQuery.fancybox('%3Cimg%20src=%5C'http://a7.sphotos.ak.fbcdn.net/hphotos-ak-ash4/239_11624132909_815407909_420420_5659_n.jpg%5C'%20height=%5C'453%5C'%20width=%5C'604%5C'%20/%3E');%20//window.open('http://www.facebook.com/photo.php?fbid=11624132909&set=a.11623722909.18690.815407909&type=1');%22%20style=%22cursor:pointer;background:%20url(http://photos-g.ak.fbcdn.net/hphotos-ak-ash4/239_11624132909_815407909_420420_5659_s.jpg)%20no-repeat;%20height:65px;width:90px;border:1px%20solid%20gainsboro;padding:2px;%22%3E%3C/div%3E%3C/div%3E%3C/div%3E%3C/td%3E%3C/tr%3E%3C/table%3E",
    "info": null,
    "profile_streams": [
        {
            name: "Stream",
            stream: "profile_feed"
        },
        {
            name: "Tagged",
            stream: "profile_tagged"
        }
    ],
    "profile_actions": [
        {
            "name": "Follow",
            "action": "follow",
            "can_message": false,
            "message_prefix": ""
        },
        {
            "name": "DM",
            "action": "dm",
            "can_message": true,
            "message_prefix": "d "
        },
        {
            "name": "Reply",
            "action": "reply",
            "can_message": true,
            "message_prefix": "@"
        }
    ]
}
```

The `profile_streams` array returns a list of other possible streams that can be retrieved for the current profile. These can be used with the [GetStream](GetStream.md) call. For example:
http://sendible.com/api/v0/stream-fetch?handle=xxxx&stream=profile_tagged&account_id=xxxx

  * `application_id`: Your application id from http://sendible.com/developers.
  * `account_id`: The account ID for this stream.
  * `handle`: The user's profile identifier. This is returned by the [GetStream](GetStream.md) call in the `uid` field.
  * `stream`: The value returned in the `stream` field within the `profile_streams` array.

#### Error Response: ####
```
<error>
<type>InvalidUsernamePassword</type>
<message>Username/password is invalid.</message>
</error>
```