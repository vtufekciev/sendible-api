To find out which users a particular entity is shared with (or not shared with), make an authenticated GET request..

#### URL: ####
http://sendible.com/api/v0/users-shared.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `type`: The type of list to retrieved. E.g. `shared` or `unshared`. `unshared` will return the list of users who have not had this entity shared with them. `shared` will return the list of users who have had this entity shared with them.
  * `entity`: The entity type. E.g. `service`.
  * `entity_identifier`: The entity ID. E.g. the ID of the account.


#### Authentication: ####
Basic authentication with username and password or remote API key/access token belonging to the Sendible user.

#### Success Response: ####
```
{
    "users": [
        {
            "login": "acme222",
            "id": 122918,
            "fullname": "acme222"
        },
        {
            "login": "adamsendible1",
            "id": 97930,
            "fullname": "adamgigi"
        },
        {
            "login": "alexsendible",
            "id": 99583,
            "fullname": "Alex "
        },
        {
            "login": "alextest",
            "id": 112468,
            "fullname": "Alex Test"
        },
        {
            "login": "alextest11_OLD",
            "id": 112476,
            "fullname": "Alex Test"
        },
        {
            "login": "anky",
            "id": 59119,
            "fullname": "Ankit Shah"
        },
        {
            "login": "sendibleapprove1",
            "id": 95285,
            "fullname": "App1"
        },
        {
            "login": "clairevh",
            "id": 123073,
            "fullname": "Claire Van Hespen"
        },
        {
            "login": "foo5432reib",
            "id": 122976,
            "fullname": "foo5432reib"
        },
        {
            "login": "scottss",
            "id": 115727,
            "fullname": "Getsyncd"
        },
        {
            "login": "722productions",
            "id": 56929,
            "fullname": "Jason Nelson"
        },
        {
            "login": "johnsendible",
            "id": 116321,
            "fullname": "John"
        },
        {
            "login": "johntest1",
            "id": 121688,
            "fullname": "John Test 1"
        },
        {
            "login": "johntest2",
            "id": 121689,
            "fullname": "John Test 2"
        },
        {
            "login": "johnai",
            "id": 129372,
            "fullname": "JohnA"
        },
        {
            "login": "johnb",
            "id": 129373,
            "fullname": "JohnB"
        },
        {
            "login": "johnc",
            "id": 129374,
            "fullname": "JohnC"
        },
        {
            "login": "johndaaa",
            "id": 129375,
            "fullname": "johnD"
        },
        {
            "login": "johne",
            "id": 129376,
            "fullname": "JohnE"
        },
        {
            "login": "johnny",
            "id": 77515,
            "fullname": "Johnny Costello"
        },
        {
            "login": "johntestx",
            "id": 130657,
            "fullname": "JohnTestX"
        },
        {
            "login": "jondarrer",
            "id": 79989,
            "fullname": "Jonathan Darrer"
        },
        {
            "login": "kimdenmark",
            "id": 122441,
            "fullname": "Kim "
        },
        {
            "login": "kimsendible",
            "id": 122442,
            "fullname": "Kim "
        },
        {
            "login": "mesiand",
            "id": 114220,
            "fullname": "mesian morison"
        },
        {
            "login": "newjohn05603",
            "id": 123100,
            "fullname": "NewJohn05603"
        },
        {
            "login": "newjohn123",
            "id": 122970,
            "fullname": "newJohn123"
        },
        {
            "login": "newjohn48746",
            "id": 123120,
            "fullname": "NewJohn48746"
        },
        {
            "login": "newjohn89379",
            "id": 123127,
            "fullname": "NewJohn89379"
        },
        {
            "login": "nowy123",
            "id": 123152,
            "fullname": "nowy123"
        },
        {
            "login": "PeterSouris",
            "id": 122146,
            "fullname": "Peter Souris "
        },
        {
            "login": "RichardCrow",
            "id": 122147,
            "fullname": "Richard Crow"
        },
        {
            "login": "SendibleSocialChannels",
            "id": 137532,
            "fullname": "Sendible"
        },
        {
            "login": "sendtest1",
            "id": 129377,
            "fullname": "Sendible Test"
        },
        {
            "login": "sendible222",
            "id": 110009,
            "fullname": "sendibltetest"
        },
        {
            "login": "testing1111",
            "id": 129381,
            "fullname": "test"
        },
        {
            "login": "xpxpxp",
            "id": 122051,
            "fullname": "Test User"
        },
        {
            "login": "xpxaaaaaa",
            "id": 122068,
            "fullname": "Test User"
        },
        {
            "login": "xpxaaaaaa4",
            "id": 122071,
            "fullname": "Test User"
        },
        {
            "login": "xpxaaaaaa45",
            "id": 122074,
            "fullname": "Test User2"
        },
        {
            "login": "xpxaaaaaa46",
            "id": 122083,
            "fullname": "Test User3"
        },
        {
            "login": "tomboyd",
            "id": 120002,
            "fullname": "Tom Boyd"
        },
        {
            "login": "ujyt123",
            "id": 122973,
            "fullname": "ujyt123"
        },
        {
            "login": "roo98766",
            "id": 122977,
            "fullname": "updateJohn91858"
        },
        {
            "login": "vishalp",
            "id": 96391,
            "fullname": "Vishal Pindoriya"
        },
        {
            "login": "wpjr2011",
            "id": 74797,
            "fullname": "Wally P"
        },
        {
            "login": "xxxxxse",
            "id": 120337,
            "fullname": "xxxx"
        },
        {
            "login": "xxxxxse",
            "id": 120338,
            "fullname": "xxxx"
        }
    ]
}
```