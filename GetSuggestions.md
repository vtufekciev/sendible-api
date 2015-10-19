The user content endpoint is a read-only resource used for receiving content recommendations for a given user or topic. It returns a JSON array of content items represented by JSON objects as detailed below.

#### URL: ####
http://sendible.com/api/v2/suggested_content.json

#### HTTP Methods: ####
GET

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `topics`: Optional. Set this parameter to return results for a set of topics, separated by commas. These must be valid topics and are case sensitive, returned by this call: [GetSuggestedTopics](GetSuggestedTopics.md)

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
  "items": {
    "results": [
      {
        "body": "American Veteran Fighting ISIS in Syria: 'I'm Ready to Stay Until the End'\nISTANBUL, Turkey\u2014Jordan Matson, a U.S. military veteran who quit his job to fight the Islamic State, was wounded in battle shortly after getting to Syria.\nBut rather than discourage other Americans from coming to the front lines, the 28-year-old from Wisconsin instead turned to Facebook, becoming an intermediary between Kurdish forces and Americans eager to join the battle against jihadi militants.\n\"I'm ready to stay until the end,\" Matson said via Skype, wearing fatigues and a Kurdish scarf draped across his shoulders.\nWhile ISIS recruitment efforts of Westerners is well-documented, less has been written about the other side.\nEver since reports about him began circulating early this month, Matson said many fellow U.S. veterans have reached out asking how they too can come to Syria to fight.\n\"Veterans did their tours of Iraq. To watch Mosul fall \u2014 and to see all that we paid to bring democracy to Iraq fall apart \u2014 is hard,\" Matson said from a Kurdish military base in northeastern Syria. \"Many other veterans are upset.\"\nThe conflict that began in Syria and has now spread into Iraq has been brutal. Tens of thousands have been killed, and hundreds of thousands of men, women and children are on the run. The militant group is holding thousands hostage inside ISIS territory, where it has revived the practice of slavery. Prospects for any rescue are bleak.\nMatson recently posted a message to his Facebook page, urging prospective fighters to \u201cbe patient as the outcry to join the fight is immense.\u201d\nCurrently, there are only four known Americans fighting alongside the Kurds in northeastern Syria, according to Kurdish journalist Sinan Cudi. But Matson expects many more to be on their way. \u201cThey're coming,\u201d he said.\nJordan Matson, an American veteran, fighting ISIS on the side of the Kurds in Syria\nImage: Sinan Cudi\nMatson had been working odd jobs in Wisconsin \u2014 most recently for a food packaging company \u2014 when ISIS began its rampage through northern Iraq.\n\u201cThey were killing Christians, so many innocent people, driving minorities out of their homes,\u201d he recalled.\nWhen ISIS beheaded the American journalist James Foley in August, Matson decided to go to Syria to fight the radical group. And getting there was surprisingly easy. Matson simply combed the Internet to find groups he could join in the battle and eventually settled on the Kurdish group known as YPG.\nThe YPG had been fighting to push the radical militants from the Kurdish northeast of the country since 2013. Since mid-September, its fighters, who number both men and women, have gained international attention by taking a stand against the more heavily armed ISIS fighters in the town of Kobani.\nWith just a pair of boots, a change of clothes and five sticks of deodorant in his bag \u2014 \u201cI wanted to be prepared,\u201d he said \u2014 Matson boarded a flight from Chicago to Istanbul, the gateway for many foreigners who have crossed into Syria to fight.\nRather than continue to the southern province of Hatay, a popular destination for prospective jihadis, he set off for the southeastern city of Diyarbakir, the so-called Kurdish capital of Turkey. Once there, he met the YPG contacts he had met online, who took him across the border \u2014 and into the war.\nSoon after, Matson was struck by an ISIS mortar which caused minor injuries to his foot and eye and was brought to a hospital. Despite the language barrier, Kurdish families came to check on him and other wounded soldiers every day, eating dinner with them as if they were part of \u201ca big, extended family.\u201d\n\"There's a lot of love and compassion,\" he said, pointing out that, at one point, a fellow fighter, who is Muslim, brought him to church in town so he could pray.\nMany Kurds are Sunni Muslims, as are the members of ISIS, but they practice a less radical form of the faith.\nMatson has mostly recovered from his injuries and now spends much of his time communicating with hopeful recruits.\nJordan Matson, a U.S. military veteran, is fighting ISIS in Syria on the side of the Kurds.\nImage: Sinan Cudi\nOther Americans, however, appear to have found their way to the front without his help.\nA man named Brian Wilson recently identified himself to a Reuters photographer in the Syrian town of Kamishli as a U.S. veteran from Ohio now fighting with the YPG. Jeremy Woodard, a 28-year-old veteran from Mississippi who said he had served tours in both Iraq and Afghanistan, told CBS News that he thought that by joining the fight against ISIS, he might inspire other foreigners to follow his example.\nMany of the inquiries Matson is fielding come from veterans of the Iraq war. Matson did not see any combat himself, having left the military early for \"personal reasons,\" he said, without elaborating.\nMany of the inquiries Matson fields comes from veterans, but a Daily Beast report suggests that Matson's own departure from the military was troubled. During a traffic stop in 2012, in which a gun was found in his car, Matson told police that he suffered from post-traumatic stress disorder and had been \"'railroaded out' of the military in 2007.\"\nSince coming to Syria to fight, Matson's Facebook page has blown up with fan mail, with Americans and foreigners alike congratulating him on fighting ISIS. Even his mother appears pleased.\nI \"always knew deep in my heart that God would do something amazing with you,\" she recently wrote. \"God has revealed to you his purpose and plan, you answered the call, he has equipped you for this journey and in doing so I know he has filled you with his peace. Carry on son, I love you!!\"\nMashable is a leading source for news, information and resources for the Connected Generation. Mashable reports on the importance of digital innovation and how it empowers and inspires people around the world. Mashable's record 40 million unique visitors worldwide and 19 million social media followers are one of the most influential and engaged online communities. Founded in 2005, Mashable is headquartered in New York City with an office in San Francisco.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/8be604afcbd84380b803313f2c1fbdc3_medium.png"
          }, 
          "original": {
            "size": [
              1200, 
              627
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/8be604afcbd84380b803313f2c1fbdc3.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/8be604afcbd84380b803313f2c1fbdc3_thumb.png"
          }
        }, 
        "index": 0, 
        "published": 1413992074, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=87&sm=1&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9tYXNoYWJsZS5jb20vMjAxNC8xMC8yMi9hbWVyaWNhbi12ZXRlcmFuLWZpZ2h0aW5nLWlzaXMtc3lyaWEvIg.2o_ie1ScohHafbplfcpSNL9W1f4&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=0", 
        "source": "http://mashable.com/", 
        "title": "American Veteran Fighting ISIS in Syria: 'I'm Ready to Stay Until the End'", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=87&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9tYXNoYWJsZS5jb20vMjAxNC8xMC8yMi9hbWVyaWNhbi12ZXRlcmFuLWZpZ2h0aW5nLWlzaXMtc3lyaWEvIg.2o_ie1ScohHafbplfcpSNL9W1f4&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=0"
      }, 
      {
        "body": "Cuba has sent a second group of medical staff to West Africa to help fight the Ebola outbreak.\n\nThe 83 doctors and nurses will treat Ebola patients in Liberia and Guinea.\n\nAnother contingent of 165 Cuban healthcare professionals travelled to Sierra Leone a few weeks ago.\n\nCuba is now the biggest single provider of healthcare workers to the Ebola crisis in West Africa, more than the Red Cross or richer nations, the World Health Organization says.\n\n\"Cuba has provided the numbers and the people,\" said Jose Luis Di Fabio, the WHO representative on the Caribbean island.\n\n\"There are more human resources from Cuba than from many, many NGOs [non-governmental organisations] put together.\"\n\nThe epidemic has killed more than 4,500 people in West Africa.\n\nThe Red Cross, which is trying to tackle Ebola in Sierra Leone, has said the scale of the outbreak is so bad that it is having to retrieve more than 100 corpses a day.\n\n\"We cannot see our brothers from Africa in difficult times and remain there with our arms folded,\" the Cuban Ambassador to Liberia, Jorge Lefebre Nicolas, told Reuters news agency.\n\nA jet from the national airline Cubana carrying 51 medical personnel touched down on Wednesday morning at the Roberts International Airport outside the Liberian capital, Monrovia, Reuters reports.\n\nCuba has been praised for its response to the Ebola crisis, including by the United States.\n\nDespite America's frosty relations with the Communist island, US Secretary of State John Kerry cited Cuba as an example of a small nation which sent more than larger, richer states.\n\nIts response has also won plaudits from humanitarian workers who say the international community's reaction has been lacking.\n\nThe BBC's Will Grant in Cuba says that, for President Raul Castro, this has also been an opportunity to build on the island's long-standing tradition of humanitarian aid to Africa.\n\nThe president shook the hands and embraced the 83 doctors and nurses who waved Cuban flags as they boarded the plane for West Africa, our correspondent adds.\n\nMore Cuban medics have been trained to travel there.", 
        "images": {
          "medium": {
            "size": [
              464, 
              261
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/b86cc0083d464bd799a9081007708baf.png"
          }, 
          "original": {
            "size": [
              464, 
              261
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/b86cc0083d464bd799a9081007708baf.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/b86cc0083d464bd799a9081007708baf_thumb.png"
          }
        }, 
        "index": 1, 
        "published": 1414000871, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=87&sm=1&a_id=ve1ve1de1&url_id=Imh0dHA6Ly93d3cuYmJjLmNvLnVrL25ld3Mvd29ybGQtbGF0aW4tYW1lcmljYS0yOTczMjI5MSI.r7d-okJklRtwASOyUAmvFoVtaJU&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=1", 
        "source": "http://news.bbc.co.uk/", 
        "title": "Cuba leads way on Ebola effort", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=87&a_id=ve1ve1de1&url_id=Imh0dHA6Ly93d3cuYmJjLmNvLnVrL25ld3Mvd29ybGQtbGF0aW4tYW1lcmljYS0yOTczMjI5MSI.r7d-okJklRtwASOyUAmvFoVtaJU&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=1"
      }, 
      {
        "body": "The man who shot a Canadian soldier Wednesday and then stormed Parliament before being shot dead had been attempting to get passport and then fly to the Middle East, officials said Thursday.\n\nMichael Zehaf-Bibeau had been in Ottawa since at least Oct. 2 \"to deal with a passport issue, but was hoping to leave for Syria,\" Royal Canadian Mounted Police Commissioner Bob Paulson said at a press conference. He said that the shooter's mother yesterday had told them that he was planning to go to Syria.\n\nHe said that the RCMP had been asked to do a background check on Zehaf-Bibeau, who had several low-level criminal offenses in his past but was not a national security risk.\n\nThe commissioner said that the holding up of the passport may have been a reason for the shooting.\n\n\"I think the passport figured prominently in his motives,\" said Paulson. \u201cI\u2019m not inside of his head, but I think it was central to what was driving him.\"\n\nPaulson said that Zehaf-Bibeau was not on a list of some 90 individuals whom Canadian officials earlier this month had deemed \u201chigh-risk travelers\u201d \u2014 and his passport application had not yet been rejected, as the background check process was ongoing at the time of the attack.\n\nHe said Zehaf-Bibeau, who may have had a dual citizenship with Libya, used a .30-30 Winchester lever-action gun to first shoot Cpl. Nathan Cirillo dead before driving to the Parliament building and exchanging gunfire with police and guards before being killed.\n\nDuring the briefing, police played surveillance video showing the gunman diving up to Parliament in one car, getting, out, hijacking another car which belonged to a lawmaker but only had a chauffeur inside, then continuing on to the central building where he exited the vehicle and ran inside.\n\nCanadian police confirmed Thursday that Zehaf-Bibeau was the lone gunman in Wednesday\u2019s rampage, the second attack on Canadian soldiers in three days.\n\nOn Monday, Martin Rouleau, 25, drove his car into two Canadian soldiers, killing one, in a Quebec parking lot.\n\nAfter a chase and shootout with police, Rouleau died in a hospital. Prior to the incident, Rouleau \u2014 like Zehaf-Bibeau \u2014 had his Canadian passport revoked and was being monitored by the Royal Canadian Mounted Police, according to Canadian officials.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/16ffe42fe754433eb0de3a56f1dfb934_medium.png"
          }, 
          "original": {
            "size": [
              2500, 
              2000
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/16ffe42fe754433eb0de3a56f1dfb934.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/16ffe42fe754433eb0de3a56f1dfb934_thumb.png"
          }
        }, 
        "index": 2, 
        "published": 1414096827, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=92&sm=1&a_id=tt1to1da1&url_id=.eJxtykEOgzAMBdG7sDcR0EXFbdwQgaXkJ4pdLG4PB2A7b4bDrK0huPuIX0RyHWMtQa32KwtSiAzehEGNexYuCUZ61GqC_RX3P8pTnJVaZuD5yDqfKZNeXZgwL_PnOw03g8kuOw._crEEH6uVWCizJNjJG6_-I3hb38&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=2", 
        "source": "http://nbcnews.com/", 
        "title": "Canada Gunman Was Planning to Travel to Syria: Officials", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=92&a_id=tt1to1da1&url_id=.eJxtykEOgzAMBdG7sDcR0EXFbdwQgaXkJ4pdLG4PB2A7b4bDrK0huPuIX0RyHWMtQa32KwtSiAzehEGNexYuCUZ61GqC_RX3P8pTnJVaZuD5yDqfKZNeXZgwL_PnOw03g8kuOw._crEEH6uVWCizJNjJG6_-I3hb38&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=2"
      }, 
      {
        "body": "Even if you\u2019re only a casual internet user, chances are that by now you\u2019ve probably heard something about the movement known as Gamergate. If you\u2019re unfamiliar with what Gamergate is, we\u2019ve taken the liberty of writing up a brief summary of the movement and its goals, which we will immediately change if anything in it offends anyone who associates with Gamergate.\nWhat is Gamergate?\nGamergate is a movement of video game fans who are fighting to achieve something involving ethics in gaming journalism using reasonable, measured debate. Note, though, that should a single word of that description make members of the Gamergate movement angry or uncomfortable, we are perfectly willing to rewrite it. Please just let us know!\nWhat do members of Gamergate want?\nOne need only spend three or four hours perusing Gamergate message boards to know that the main thing members of the movement want is ethics in gaming journalism\u2014there aren\u2019t enough ethics, and so, one way or another, there will have to be more ethics. They might want other things too, but we had a hard time figuring out what they were. Again, if you\u2019re a member of Gamergate who feels like we didn\u2019t get this part exactly right, please just tell us what you want added or removed, and you can consider it done. We don\u2019t want any trouble.\nWhat\u2019s \u201cwrong\u201d with Gamergate?\nCoverage of Gamergate by certain media outlets ***that we do not necessarily agree with*** has focused on a long series of female game designers and critics who have been forced to flee their homes after individuals identifying with the Gamergate movement bombarded them with a significant amount of online harassment, followed by explicit threats to rape and murder them. This has led many to decry Gamergate as somehow misogynistic or violent, and is an aspect of this whole issue we\u2019d readily omit here if members of the movement told us to.\nBecause it\u2019s only one side of the story! The rape threats and hate speech are coming from only one, extremely vocal, extremely visible faction within Gamergate. These radical individuals distract from the main message of Gamergate. It is important to remember that the members of Gamergate, only some of whom threaten to rape and murder women, are simply fighting for ethics in gaming journalism.\nHow is Gamergate answering its critics?\nIn order to clarify their message, members of Gamergate have seen to it that any individual who unfairly singles out the violent and bigoted aspects of the movement for criticism immediately becomes the target of sustained online harassment. Needless to say, we don\u2019t mean for that last sentence to sound like a criticism of Gamergate. We\u2019d even go so far as to say that anybody critical of Gamergate probably had it coming, if that is better.\nListen: If you\u2019re thinking about targeting the authors of this article, or mounting a campaign to get funding for this website pulled, please reconsider, and instead, just tell us how to make this thing look the way you want it to look.\nIs Gamergate a vast, complex, and diverse community?\nYes! It is not composed, as the mainstream media would lead you to believe, solely of white male trolls. It also has female trolls. It has African-American trolls and Asian trolls, gay trolls and straight trolls. In fact, Gamergate is all about the inclusion of anyone\u2014regardless of gender, race, or sexual orientation\u2014whose views on video games and how we should think about them conform exactly to those of the movement at large.\n\u2014\u2014\u2014\nIs that right? If you are a member of Gamergate, let us know if that is not right, or if any of that made you angry. We\u2019ll change it right away. We want to accurately reflect your dedication to something involving ethics in journalism. We want to tell the world about what you are trying to build. Or destroy. We don\u2019t know. It\u2019s been a bit tricky to piece together what it is you\u2019re trying to do and how you\u2019re trying to do it.\nWe would hasten to add, before our Twitter feed is turned into a hellish garbage dump for the worst discussion ever conducted on the internet, that these women driven from their homes, these journalists targeted by hate campaigns, and these websites financially punished for their dissent are all unfortunate victims of a few fringe individuals within Gamergate. That these are the movement\u2019s only tangible achievements so far does not change the fact that this is, at its core, a concerned community dedicated to having a reasonable discussion about ethics in journalism.\nAnd that\u2019s the best part of the whole thing, right? That Gamergate, as a legitimate movement arguing in good faith, can accept criticism and dissent without resorting to vitriolic censorship or threats of violence.\nUnless you guys aren\u2019t into that. If not, then that\u2019s totally fine. Just look this whole thing over and tell us if there\u2019s anything we should change. Email all of your demands to Gamergate@ClickHole.com. We\u2019ll get on it right away.\nLike you, we value ethics in journalism, and will alter our content in whatever way you feel best supports those values.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/26cac46a20eb43109541b44565b584b6_medium.png"
          }, 
          "original": {
            "size": [
              1200, 
              675
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/26cac46a20eb43109541b44565b584b6.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/26cac46a20eb43109541b44565b584b6_thumb.png"
          }
        }, 
        "index": 3, 
        "published": 1413994876, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=tr1ca1ca1&url_id=.eJwNyTEOgDAIAMC_dMemxsnfECQtEaypKPH3euul5n6uOUfERCq0t648UbeMw4WU83Wb4XihovGo6AzWHzY-HIIhRBXEjDf5S1-ghlDmpaQP_xUhCg.GKzF9mCDy5TxIq2iP5NuIfXwtVE&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=3", 
        "source": "http://digg.com/", 
        "title": "A Summary Of The Gamergate Movement That We Will Immediately Change If Any Of Its Members Find Any Details Objectionable", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=tr1ca1ca1&url_id=.eJwNyTEOgDAIAMC_dMemxsnfECQtEaypKPH3euul5n6uOUfERCq0t648UbeMw4WU83Wb4XihovGo6AzWHzY-HIIhRBXEjDf5S1-ghlDmpaQP_xUhCg.GKzF9mCDy5TxIq2iP5NuIfXwtVE&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=3"
      }, 
      {
        "body": "The plain-looking, white device you see up there isn\u2019t a promotional flash drive Intel was giving out to conference attendees. It\u2019s actually a Bay Trail Atom PC that tips the scales at just 1.6 ounces.\n\nIt\u2019s similar to Google\u2019s Chromecast, at least in the sense that it\u2019s designed to plug into an HDMI port, can be powered via a micro USB port, and connects to the Internet via WiFi. This isn\u2019t just a dongle you can cast video to, however. It\u2019s a full-blown x86 PC.\n\nThis little fella is manufactured by the Shenzen Apec Electronics, and you can pick one up on AliExpress for around $125 including shipping. That price doesn\u2019t include an OS, but you\u2019re free to load Windows, Linux, Android, or any other Atom-friendly OS you want onto it.\n\nWhat can you cram into a PC this small? Apart from the quad-core Bay Trail processor (a 32-bit Z3735F), it\u2019s got 1GB of RAM, 16GB of storage, 802.11b/g/n and Bluetooth 4.0, and a micro SD expansion slot. A beefier model is available with a 64-bit Atom Z3735G and 2GB of RAM, but the seller doesn\u2019t have a price posted for the upgrade. Internal storage can be bumped up to 32GB, but again\u2026 no pricing.\n\nThe guts in here are similar to what you\u2019d find inside that $65 Windows tablet that popped up earlier this week. As far as why you can tack on a touchscreen display, a rechargeable battery, pre-load Windows on it, and still price the device $60 less than this PC, well\u2026 in the tech game, smaller things often cost more money.\n\nThat might not be the official explanation from Shenzen Apec, but it\u2019s certainly true in a lot of cases.", 
        "images": {
          "medium": {
            "size": [
              500, 
              280
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141217/1177b7e6a4a0440dad6b1019d68dcff7_medium.png"
          }, 
          "original": {
            "size": [
              625, 
              350
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141217/1177b7e6a4a0440dad6b1019d68dcff7.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141217/1177b7e6a4a0440dad6b1019d68dcff7_thumb.png"
          }
        }, 
        "index": 4, 
        "published": 1413577453, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=on1ca1ca1&url_id=.eJwVzFsOwjAMRNG99H8aWiGQ2E1JrNoqeSh2sbp7wuccje7EZu0VgrvPO9Exx5pDZGkajEUhWgwbjM_8Tl2-BDEd0OKwzeAkOys-pPqHghX1LJHGpyR47cdolDEucMqCVrthedyey3oP0w9ckCx2._hNDA4F5Okqg6xVsiUbW8hlVsE8&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=4", 
        "source": "http://www.geek.com/", 
        "title": "This isn\u2019t a thumbdrive, it\u2019s a PC that weighs less than 2 ounces and works in any HDMI port", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=on1ca1ca1&url_id=.eJwVzFsOwjAMRNG99H8aWiGQ2E1JrNoqeSh2sbp7wuccje7EZu0VgrvPO9Exx5pDZGkajEUhWgwbjM_8Tl2-BDEd0OKwzeAkOys-pPqHghX1LJHGpyR47cdolDEucMqCVrthedyey3oP0w9ckCx2._hNDA4F5Okqg6xVsiUbW8hlVsE8&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=4"
      }, 
      {
        "body": "According to Dr. David B Allen, a retired Cardiothoracic and Vascular Surgeon, and medical director at Cannabis Sativa Inc, we may be able to protect ourselves from the Ebola virus using cannabis. While claims like this come forward, others suggest we may not be hearing the full story when it comes to Ebola.\n\nCannabinoids may be one of the best disease fighting treatments out there. Cannabinoids refer to any of a group of related compounds that include cannabinol and the active constituents of cannabis. They activate cannabinoid receptors in the body. The body itself produces compounds called endocannabinoids and they play a role in many processes within the body that help to create a healthy environment.\n\nThis fact has led a couple of doctors to suggest that in turn cannabinoids can provide sufficient protection from viral infections.\n\n\u201cThere is good scientific evidence that cannabinoids, and in particular Cannabidiol (CBD), may offer control of the immune system and in turn provide protection from viral infections (4). Cannabis has already been recognized to inhibit fungus and bacteria and can be considered a new class of antimicrobial because of the different mechanism of action from other antimicrobials.\n\nEbola is a complex RNA viral organism that causes the cell to engulf it by pinocytosis, and then the virus hijacks the cell to replicate itself. This replication can involve many mutations in the RNA code that make it difficult to impossible to create an effective vaccine. There are U.S. Patents showing evidence that Cannabinoids have significant anti-viral activity. \u201d (source)\n\nHe states how the Ebola virus causes the cell to produce proteins that hide the virus from the immune system, which allows the RNA virus to hide the infected cell by shielding it from view from the immune system.\n\nHe adds that the cause of death by this virus is the body\u2019s own immune response to the actual viral infection itself by triggering the immune killer cells to release the cytokines they hold, which is termed a \u201cCytokine Storm.\u201d\n\nA cytokine storm forces the body into a toxic shock state, and causes small blood clots to form in all arterioles, which is called Disseminated Intravascular Coagulation (DIC).\n\nSince cannabinoids have been shown to prevent Toxic Shock as well as DIC, they could be a viable solution. Of course more testing and research would need to be done on this. Luckily something like cannabis, especially when eaten raw, does not have dangerous side effects and therefore could help in areas where Ebola is actually spreading.\n\nTo read his full article that goes into more detail and includes sources, you can click HERE.\n\nThe recent Ebola scare seems to be going viral on the internet. Anything from theories behind how to stop it to theories about it being a bio-weapon.  What\u2019s interesting is that (apparently) there are even citizens in West Africa making various claims suggesting that the only ones who\u2019ve fallen ill are the ones who\u2019ve received treatment.\n\nBeyond these claims, the internet has become flooded with potential natural cures and various ways to boost ones immune system, one of them being cannabis.\n\nThis is difficult to say. There is a lot of information going around that claim hoaxes and what not, the truth is it\u2019s tough to tell and certainly not all the pieces are put together. We\u2019re better off exploring this as if it\u2019s factual as opposed to just assuming it\u2019s a lie. But this doesn\u2019t mean jumping straight to the vaccine.\n\nIt seems claims coming from outside of the western media state that what is actually happening in areas where Ebola is more common is not quite what is being reported in the media. A man named Nana Kwame from Ghana has stated:\n\n\u201cPeople in the Western World need to know what\u2019s happening here in West Africa. THEY ARE LYING!!!\u2026. The Red Cross has brought a disease to 4 specific countries for 4 specific reasons and it is only contracted by those who receive treatments and injections from the Red Cross. That is why Liberians and Nigerians have begun kicking the Red Cross out of their countries and reporting in the news the truth.\u201d  (source)\n\nWhat\u2019s also seems to be causing much confusing is the fact that the United States government patented the Ebola virus a few years ago. You can view that here.   This is done so that governments or corporations can profit from it, like the vaccine that will be issued in a few months, for example.\n\nI personally believe if there was anything to worry about, it may be the vaccine itself. Remember what happened with the H1N1 vaccine? It was rushed to market and injured a lot of people. In terms of all of the Ebola info, I haven\u2019t found enough information on the topic to make further comments about it.\n\nThis does demonstrate one thing though, more and more people are loosing complete trust in corporate media, and it\u2019s becoming harder and harder to find real truthful information.", 
        "images": {
          "medium": {
            "size": [
              484, 
              252
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141217/d522b7ffe4dc448f91494048286dfb77.png"
          }, 
          "original": {
            "size": [
              484, 
              252
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141217/d522b7ffe4dc448f91494048286dfb77.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141217/d522b7ffe4dc448f91494048286dfb77_thumb.png"
          }
        }, 
        "index": 5, 
        "published": 1413664015, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=86&sm=1&a_id=ve1ve1de1&url_id=.eJwNzEEOhCAMBdC7uK8VM4uJt-lgVQzwDRTJ3F63b_GGw-xamHvvo0eM6i3cSnojNgvILyaeJ_dhN7H78gpvKFTbvmu1SnaIUZISziZZyEumq8Dehv5otBUk0h-i8PAADkkmbQ._Hrt3xZL8MJCKwnjRP6--33A9Q4&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=5", 
        "source": "http://collective-evolution.com/", 
        "title": "Doctor Suggests That Marijuana Can Protect You From Ebola", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=86&a_id=ve1ve1de1&url_id=.eJwNzEEOhCAMBdC7uK8VM4uJt-lgVQzwDRTJ3F63b_GGw-xamHvvo0eM6i3cSnojNgvILyaeJ_dhN7H78gpvKFTbvmu1SnaIUZISziZZyEumq8Dehv5otBUk0h-i8PAADkkmbQ._Hrt3xZL8MJCKwnjRP6--33A9Q4&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=5"
      }, 
      {
        "body": "In his book, Rich Habits -- The Daily Success Habits of Wealthy Individuals, Tom Corley outlines several habits that distinguish the wealthy from the nonwealthy.\nIt got me to think, How many people operate on autopilot and don\u2019t stop to monitor their everyday patterns? Below I've summarized 19 of his habits for success (nine culled from his book and the next 10 from his recent article in Success) plus two of my own. If you're not actively engaged in these 21 things, you are, in effect, leaving money on the table.\n1. Setting good daily habits.\nGood habits are the foundation of wealth building. The difference between successful and unsuccessful people lies in their daily habits. Simply put, successful people have many good habits and few bad ones. If you understand that your bad habits may be preventing you from becoming wealthy, that realization will be the first step in your improving your circumstances.\nIn his book, Corley invites you to take out a sheet of paper and list your bad habits in one column and then invert each one to place under a new column for good habits. It should look like this:\nBad Habit Good Habit\nI watch too much TV. I limit myself to one hour of TV per day.\nI don\u2019t remember names. I write down names and remember them.\nThen for 30 days, follow the guidance of your new good habits list. You\u2019ll be amazed at how much you can accomplish.\n2. Regularly creating goals.\nSuccessful people are goal driven. They create goals all the time. They plan their day the night before with to-do lists.\nPeople who are headed for success think for the long term. They have daily, weekly, monthly and yearly goals. But what\u2019s a goal without a plan to reach them? So not only do successful people have goals, they also come up with ways to achieve them and hold themselves accountable.\n3. Engaging in self-improvement daily.\nSuccessful people are always looking for ways to improve themselves. They read every day and are students of their profession. They don\u2019t spend their time on activities that don't bring them closer to their goals.\nI recently attended an event hosted by author Brendon Burchard, who said he consistently blocks out time to create. Successful people like Burchard know that time is too valuable a commodity to waste. They spend their time on the things that will move the needle for them in their business: Being committed to self-improvement means you engage in activities every day that will stretch you.\nSeek ways to expand your knowledge. This won\u2019t always be easy, but people grow from things that pose a challenge. Once your knowledge grows, opportunities appear.\n4. Regularly taking care of personal health.\nEach and every day successful people make an effort to eat right and exercise. Eating right is of utmost importance. Exercising daily can become a regular habit, just like taking a bath. People who exercise routinely have more energy to get things done. How are you doing in this area?\n5. Often making time for relationship building.\nPeople who are successful are other-people focused. They take time out of their day to strengthen the bonds of friendship and form long-lasting relationships with others. Networking is something they do all the time. They reach out to their contacts and look for ways to help them with no expectation of in return.\nThe most beautiful sound on Earth, I once heard someone say, is your name. So make it a goal to learn the names of every contact you meet. Aren\u2019t you impressed when someone remembers your name? I know I am. So stand out as different and start remembering names.\n6. Doing things in moderation.\nYou live in a balanced way if you do activities in moderation. This means having a balanced approach to work, eating, exercise, consuming alcohol, watching television, surfing the Internet and so forth. As a result, people will enjoy your company. If people like being around you, then you will be more apt to collaborate or find the new business partner that you need to take your business to the next level.\n7. Getting things done.\nDon\u2019t put off to tomorrow what you can do today: Accomplish things. All people have fears, but successful people push past them. They don't procrastinate. They get the important things done, no matter the cost.\nIn Rich Habits, Corley explains that when the thought of putting off something enters the mind, immediately shed notion by saying, \u201cDo it now.\u201d He says repeat these words 100 times if necessary. Just don\u2019t stop till the task is done.\n8. Keeping a positive outlook.\nConsider the most successful person you know. Is that person positive or negative? Most likely this individual is positive, enthusiastic, energetic and happy. This person chooses to see the good in others and in himself or herself. To this person, problems are just opportunities waiting to be uncovered.\nEvery day people are bombarded by news of bad deeds and doings. Successful people minimize their exposure to this type of thing and instead opt to fill their minds with positive ideas from books and magazines.\n9. Regularly saving money.\nAccording to Corley, successful individuals put away about 10 percent to 20 percent of their gross earnings in a savings, investment or retirement plan. Not everyone can afford to do so, but what percent are you putting away?\n10. Rejecting self-limiting thoughts.\nSuccessful people command their thoughts and emotions. As soon as bad thoughts intrude, they cast out anything that challenges their ability to succeed at the task at hand. They do not dwell on negative notions. Their self-talk is positive and not overly critical. They replace bad thoughts with good ones.\nBecause successful people engage in self-improvement daily and are constantly involved in positive things, they don\u2019t allow themselves time to indulge in negative emotions.\n11. Living within means.\nWealthy people avoid overspending. Among many of those struggling financially, some are living above their means. They spend more than they earn, live from paycheck to paycheck and are drowning in credit-card debt. If this is you, resolve today to turn things around for you and your family.\n12. Reading daily.\nMany successful people read 30 minutes or more every day. Reading can increase your knowledge and know-how. When you read, often you are seeking to improve yourself. This automatically sets you apart from your counterparts. You will stand out from the competition.\n13. Limiting TV watching.\nDid you know that many successful people limit the amount their TV time to one hour or less a day? How much time do you lose in front of the television that you could be spending doing something more productive?\n14. Doing more than what\u2019s required.\nSuccessful people regularly go above and beyond the call of duty at work. Even if something is not in their job description, they will volunteer to do it. Wealthy people make themselves invaluable. As an entrepreneur, you may not have a boss. But in what ways do you go above and beyond for your clients? How do you wow them?\n15. Talking less and listening more.\nWhen you listen, you learn. And as the adage goes, that\u2019s why people have two ears and one mouth. When you take the time to really pay attention to what another person is saying, it can truly help not only you but your bottom line as well. When you listen, you are in a better position to help others.\n16. Not giving up.\nDon't give up when the going gets tough. Successful people hang in there. They pivot. They try something new. They persist. They may have to change their direction, but they keep moving forward.\n17. Spending time with like-minded ones.\nThere's a saying that goes, \u201cShow me who your friends are and I\u2019ll show you who you are.\u201d I believe that. People are only as successful as those they choose to surround themselves with. Good associations can help you more quickly achieve your goals.\n18. Finding a mentor.\nMany people who have had a mentor have attributed their success to that person. Mentors can help you achieve your goals faster and keep you accountable. They can share valuable experience that can cut your learning time in half.\n19. Knowing your why.\nWhen you know why you're doing something, you will get what you what quicker than if you don\u2019t. Having a purpose is essential to being successful in business and in life. Why do you want to be successful? Why do you really want to be wealthy?\n20. Not giving fear the upper hand.\nEveryone has fears. Successful people don\u2019t allow their fears to limit or define them. Fear inevitably keeps you in the same position and stunts your growth. Recognize your fears and seek ways to overcome them. Interview someone you admire and ask that person how he or she overcame a fear or pick up an autobiography and take notes.\n21. Upgrading skills.\nIf you want to get ahead, there\u2019s only one way to do it: Become better at something than you are today. What's the one thing you can focus on for the next 30 days that will catapult you to rock-star status in your industry? Focus your attention on that. I heard John Lee Dumas from Entrepreneur on Fire define \"FOCUS\" like this: Follow one course until success. Will you?", 
        "images": {
          "medium": {
            "size": [
              500, 
              319
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141217/03bba1621d1840d78b0733cfab6b8cc2_medium.png"
          }, 
          "original": {
            "size": [
              610, 
              390
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141217/03bba1621d1840d78b0733cfab6b8cc2.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141217/03bba1621d1840d78b0733cfab6b8cc2_thumb.png"
          }
        }, 
        "index": 6, 
        "published": 1413586800, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=on1ca1ca1&url_id=Imh0dHA6Ly93d3cuZW50cmVwcmVuZXVyLmNvbS9hcnRpY2xlLzIzODYzMCI.uatFFGmUaG6alNq9gxGQlI9rrxE&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=6", 
        "source": "http://www.entrepreneur.com/", 
        "title": "21 Ways to Achieve Wealth and Success", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=on1ca1ca1&url_id=Imh0dHA6Ly93d3cuZW50cmVwcmVuZXVyLmNvbS9hcnRpY2xlLzIzODYzMCI.uatFFGmUaG6alNq9gxGQlI9rrxE&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=6"
      }, 
      {
        "body": "Ebola has come to be described in horror-movie terms as an affliction, in the words of the journalist David Quammen, that \u201cseems to kill like the 10th plague of Egypt in Exodus \u2014 the one inflicted by an angel of death.\u201d With a mortality rate as high as 90 percent, it kills painfully and swiftly, with a seemingly remorseless calculus. There is even an article on the website of the Centers for Disease Control and Prevention that compares Ebola to the ghastly scourge in \u201cThe Masque of the Red Death,\u201d the Edgar Allan Poe story that begins: \u201cThe \u2018Red Death\u2019 had long devastated the country. No pestilence had ever been so fatal, or so hideous.\u201d\n\nIn \u201cEbola: The Natural and Human History of a Deadly Virus,\u201d Mr. Quammen puts the frightening reality of Ebola \u2014 and the heightened language and hyperbole surrounding it \u2014 into perspective. This slender book is an expanded extract from his 2012 book \u201cSpillover: Animal Infections and the Next Human Pandemic,\u201d and it does a nimble job of situating this year\u2019s unnerving events in historical context, going back to the first recorded occurrence of the virus in 1976 and chronicling the scientific and medical efforts to understand it since.\n\nAs he did in earlier natural history books like \u201cThe Song of the Dodo\u201d and \u201cMonster of God,\u201d Mr. Quammen combines on-the-ground reporting with research and interviews to give the reader a sharp-edge understanding of the subject at hand: what is known, what is not known and what may be in dispute. His book, like most writing about Ebola, is deeply unsettling, but it\u2019s also sober minded, and in this respect, a standout in the floodlet of Ebola books, many of them quickie scare guides and medical thrillers (with portentous titles like \u201cEbola: The Final Plague,\u201d \u201cEbola: Be Afraid, Be Very Afraid,\u201d \u201cEbola: The Preppers Guide to Surviving Ebola,\u201d \u201cThe Trojan Virus: An Ebola Bioterrorism Thriller\u201d and \u201cThe Ebola Conspiracy\u201d), which seem intended to exploit public fears.\n\nIn these pages, Mr. Quammen takes Richard Preston \u2014 the author of the 1994 best seller \u201cThe Hot Zone\u201d \u2014 to task for his melodramatic approach to the subject, writing that readers should not take Mr. Preston\u2019s lurid descriptions of Ebola\u2019s consequences literally \u2014 liquefying organs until \u201cpeople were dissolving in their beds\u201d or causing victims to \u201cweep blood.\u201d (In a recent interview with The New York Times, Mr. Preston said he now wants to update his book and make \u201cthe clinical picture of the virus more clear and accurate.\u201d)\n\nMr. Quammen \u2014 like the journalist Laurie Garrett in her illuminating and encyclopedic book \u201cThe Coming Plague\u201d \u2014 shows in these pages that the reality of the virus is horrifying without any apocalyptic embellishment. He writes that experts \u201caren\u2019t sure exactly how the virus typically causes death\u201d; rather, multiple causes \u2014 including liver failure, kidney failure, breathing difficulties, diarrhea \u2014 seem to converge in \u201can unstoppable cascade.\u201d The \u201cidea of immune suppression by ebolaviruses has also appeared lately in the literature,\u201d he says, \u201calong with speculation that it might allow catastrophic overgrowth of a patient\u2019s natural populations of bacteria, normally resident in the gut and elsewhere, as well as unhindered replication of the virus itself.\u201d\n\nMuch of this book reads like a detective story, tracing the intrepid efforts of microbe hunters to understand how this dangerous virus works \u2014 the dynamics of transmission, the geographical pattern of outbreaks \u2014 and possible approaches to treatment. There are some harrowing accounts of forays by scientists into disease-ridden (and cobra-infested) bat caves in Uganda, and an equally chilling story about an infectious-disease research scientist who accidentally stuck herself with a syringe that she\u2019d been using to inject Ebola-ridden mice.\n\nOver the years, considerable attention has been devoted by scientists to unraveling the mystery of where the virus lurks when it is not infecting humans, i.e., an animal host or reservoir, where it can exist more or less benignly. The chief suspected reservoirs, Mr. Quammen says, are certain types of fruit bat, which are present in parts of Central and West Africa. The diversity of bats (\u201cone in every four species of mammal is a bat,\u201d he writes), \u201ctheir ancientness\u201d (they evolved \u201cto roughly their present form about 50 million years ago\u201d) and their abundance in large, intimate communities, he argues, might have contributed to their capacity to host a wide variety of viruses, just as their migratory habits (some journey as much as 800 miles between their summer and winter roosts) might have increased \u201cthe likelihood that they, or the viruses they carry, will come in contact with humans.\u201d\n\nWhy do \u201czoonoses\u201d (animal infections that jump over into humans, like Ebola, SARS, AIDS, Lyme disease, West Nile fever, swine flu, bird flu) seem to be more and more common? Mr. Quammen suggests that when humans \u201cencroach upon the host populations\u201d of a pathogen \u2014 \u201chunting them for meat, dragging or pushing them out of their ecosystems, disrupting or destroying those ecosystems\u201d \u2014 \u201cour action increases the level of risk.\u201d As a veterinary disease ecologist named Jon Epstein observes, \u201cIt increases the opportunity for these pathogens to jump from their natural host into a new host.\u201d\n\nIn some cases, the microbe remains benign in the new host as it was in the old one. In other cases (like HIV), the pathogen \u2014 especially RNA viruses given to high rates of mutation and replication \u2014 not only gets a foothold in the new host, but also adapts and evolves and causes serious illness.\n\nAn important study published by the journal Science in August, Mr. Quammen says, addressed the Ebola virus variant involved in this year\u2019s outbreak, which is the worst in the history of the disease. The study, he writes, indicated that \u201cthe virus was mutating prolifically and accumulating a fair degree of genetic variation as it replicated within each human case and passed from one human to another.\u201d\n\nThe high rate of mutations in the virus suggest \u201cthat continued progression of this epidemic could afford an opportunity for viral adaptation,\u201d it said, \u201cunderscoring the need for rapid containment.\u201d Or, in Mr. Quammen\u2019s words, \u201cThe higher the case count goes, the greater the likelihood that Ebola virus as we know it might evolve into something better adapted to pass from human to human, something that presently exists only in our nightmares.\u201d\n\nAs for our still highly provisional scientific understanding of ebolaviruses, Mr. Quammen reminds us that it \u201cconstitutes pin pricks of light against a dark background.\u201d", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/e0885aa39a584c6d9e0658ec05192bf2_medium.png"
          }, 
          "original": {
            "size": [
              1050, 
              591
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/e0885aa39a584c6d9e0658ec05192bf2.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/e0885aa39a584c6d9e0658ec05192bf2_thumb.png"
          }
        }, 
        "index": 7, 
        "published": 1414006842, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=93&sm=1&a_id=tt1to1da1&url_id=Imh0dHA6Ly93d3cubnl0aW1lcy5jb20vMjAxNC8xMC8yMy9ib29rcy9lYm9sYS1hLWhpc3RvcnktYnktZGF2aWQtcXVhbW1lbi5odG1sIg.K_rt0I0Sjlm6E3Yai1uG0znX-hs&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=7", 
        "source": "http://nytimes.com/", 
        "title": "Books of The Times: \u2018Ebola,\u2019 a History by David Quammen", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=93&a_id=tt1to1da1&url_id=Imh0dHA6Ly93d3cubnl0aW1lcy5jb20vMjAxNC8xMC8yMy9ib29rcy9lYm9sYS1hLWhpc3RvcnktYnktZGF2aWQtcXVhbW1lbi5odG1sIg.K_rt0I0Sjlm6E3Yai1uG0znX-hs&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=7"
      }, 
      {
        "body": "Nicki Minaj's eyeliner is a precision event, a marvel, as if drawn on by the kind of pre-programmed robot arm used for laparoscopic surgeries. It is a peacock navy color, dark and shiny and full, extending maybe a not-outrageous half centimeter up from the top lid, extending an additional still-not-crazy three centimeters outward past where her eyes end. Her eyelashes are even and delicate, like wisps from a dandelion, and I can't recall if I've ever seen her without prosthetic versions. I have had plenty of time to search my memory, though, because here on this couch, in this room, during this interview, with me sitting next to her, Nicki Minaj has fallen asleep.\n\nWe are at Barclays Center in one of the dressing rooms, which are low, low beneath Brooklyn; most are named after streets and neighborhoods in the borough. During the rehearsals for Fashion Rocks, the New York Fashion Week concert fund-raiser, the halls were filled with publicists and escorts who had to pretend not to be dazzled by those they were escorting. Minaj had walked in a few minutes before, tiny next to her assistant and her muscle, wearing black sunglasses, a trucker hat cocked to the side, and a T-shirt with the periodic-table box for carbon. She had been led straight into the DeKalb dressing room, named for the street that bisects a couple of local neighborhoods now populated by yuppies but that still contain housing projects. Her smile is a warm sun. As is this room. The temperature in here has been set to about 300 degrees, at Nicki's request. She says she gets cold a lot.\n\nNext door to her is the Canarsie dressing room\u2014I actually grew up in Canarsie; it's still a dump\u2014and inside is Usher, who at the MTV Video Music Awards last month slapped Nicki's ass and continues to slap it endlessly in GIFs all over the Internet. Nicki was the star of the VMAs that night. Her hot, humpy performance of \"Anaconda\" was part of a medley, and it was followed by a quick costume change that didn't quite reach completion: She had to pinch the two breast-covering flaps of her black dress closed, because her cue for the finale of the opener, \"Bang Bang,\" with Jessie J and Ariana Grande, came before she could zip. She power-walked in like a boss, joining the other two onstage, both of them so skinny and with such rough angles and straight edges and reaching so hard for some soul. Nicki destroyed them.\n\nThis is what she does. She takes a pretty good song, waits until you are popping along to it, then a little longer, until it feels repetitive and you start to see through to its flaws, and then boom, she comes in and makes it a completely different song\u2014a better song. She is the best part even of great songs; her featured verse on Kanye West's \"Monster\" is the best of several, including ones by Jay Z and Rick Ross. She did that song because she was asked and because \"Kanye's a genius.\" She did \"Bang Bang\" because she \"knew it would be big.\"\n\nIn the dressing room on the other side of Nicki's, the Empire, named after a boulevard in Brooklyn that sounds regal but is even rougher than Canarsie ever was, is J.Lo. I could write a dissertation about the two seconds during which MTV caught J.Lo watching Nicki do \"Anaconda\" at the VMAs. Perhaps J.Lo, in those seconds, stares at Nicki and considers her own youth, and also that this is what she has wrought, that back when she brought this whole butt thing into the mainstream all those years ago, she went out of her way to be discreet, to keep us wanting more, to never let us look her ass directly in its eye, that it was an ass of implication and innuendo\u2014that, if she may, she made asses safe for the white folks at home in a way they never had been before. Who knew that just giving the people what they wanted would yield such success? In those two seconds, J.Lo's look is a mixture of pride and despair.\n\nIt has been counterpointed to me that perhaps J.Lo was just thinking of how far we'd all come, that now we can all celebrate our asses. I don't know; maybe if she didn't have a new album out, I'd agree. Contact me to debate this; I will make myself available. I want to talk about asses so much. I want to know what it is we're telling the world when we use our asses in the way that Nicki has been using her ass\u2014when they are not the accent in a video but the point of it.\n\nAnd most of all, of course, I want to know Nicki's thoughts on this. I was awake there in the DeKalb, and I had questions. She was asleep, which was fine, I suppose, because she didn't appear to have answers, anyway.\n\nThe Versus Versace party she'd attended the night before our interview had yielded a plastic case filled with M&M's\u2014an odd party favor, something I've received at bar mitzvahs. She pulled it out of her purse as we talked in the basement of Barclays, and this would be my only indication that she recognized she needed a boost. The case was taped closed, so I offered to open it for her; her nails, a pointy taupe manicure, were making it hard. We ate some together, and she noticed that they each had the Versus lion insignia on them. \"Isn't that crazy,\" she said, impressed.\n\nShe's into branding these days, particularly her own. In the \"Anaconda\" video, there are no fewer than five products placed prominently for advertising: her Beats by Dre speakers imprint and her Moscato but also a Victoria's Secret bra, some Air Jordans, and a baffling \"teatox\" drink called MateFit (dialysis machine sold separately). It's not exactly seamless integration, and at times it is so overt that it feels like a comment on the culture of branding, maybe some poignant thought about sex and consumerism?\n\nNope. \"My management team has a division that has a guy that his main focus is to go out there and find new brands for me to do business with or to find brands that would like to be in our videos and contribute to our budget,\" she says. It's like a Kickstarter, but for a multi-millionaire.\n\nShe was not born wealthy. Nicki, 31, grew up in Queens and attended LaGuardia, the high school from Fame. She says her father once tried to burn down her house while her mother was inside. She did odd jobs after school: She was a customer-service rep for a while, but that didn't go great. \"I like dealing with people, but I don't really like a lot of bullshit, so maybe customer service wasn't the best job for me.\" She was fired from a waitressing job at a Red Lobster after she followed a couple who had taken her pen into the parking lot and then flipped them the bird. I asked her if it was a special pen. \"No,\" she said. \"It was the principle.\"\n\nShe came to prominence in outsize, italic, caps-lock, Technicolor exaggeration\u2014pink wigs, outrageous outfits, eyelashes that were a comment about eyelashes. She had different personas\u2014alter egos, she called them\u2014with names and backstories. She did funny accents and was willing to make herself beautiful, then grotesque, then absurd, then back again. And here she is now, demure by comparison, just plain old black extensions, just a T-shirt about carbon.\n\n\"I always thought that by the time I put out a third album, I would want to come back to natural hair and natural makeup,\" she told me. \"I thought, I will shock the world again and just be more toned down. I thought that would be more shocking than to keep on doing exactly what they had already seen.\"\n\nShe no longer feels as if she needs to hide behind outrageousness. This next chapter is about success. Nicki Minaj is rap's first and only female mogul, having parlayed all your ogling into a spot on Forbes's Cash Kings list\u2014the only person of our gender paid well enough to be so honored. She is the top-charting woman in rap, a top-charting rapper in general, and a crossover phenomenon who can go back and forth between hip-hop and pop the way Taylor Swift can no longer go back and forth between country and pop.\n\nA few days earlier, she'd been in Los Angeles finishing up her third album, The Pinkprint, out this month, and she's changed things \"a billion times\" because she's a perfectionist. Her first two albums were big hits, platinum sellers. Already The Pinkprint has yielded a chart-topping single and an unstoppable meme\u2014the \"Anaconda\" cover art features Nicki, pants nowhere in sight, squatting, photographed from behind\u2014but also a quieter Nicki, and certainly a more tired one. She can't be baited into talking shit about anyone anymore; she answers questions simply and succinctly.\n\nNow that we have charted her rise as a cultural force, it is time to ask Nicki exactly what she's trying to say. If the \"Anaconda\" cover is the autumn of her flamboyance, it is time to get what we've wanted all along: an explanation of what exactly is going on here, which is something I will ask her the minute she wakes up.\n\nTo be completely accurate, she never fell into actual REM sleep during our interview, but at four separate times she dozed off, her head jerking awake at just the moment it had started to dip. In between, she was what I could call low-key and reserved, because I am generous, but the picture looked like this: those eyelids, falling, falling over eyes that would cross momentarily, closing for a moment but staying too long\u2014a blink that lasted a few blinks longer than a blink.", 
        "images": {
          "medium": {
            "size": [
              96, 
              96
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/1058a31ac21249959b836ac6815631ad.png"
          }, 
          "original": {
            "size": [
              96, 
              96
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/1058a31ac21249959b836ac6815631ad.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/1058a31ac21249959b836ac6815631ad_thumb.png"
          }
        }, 
        "index": 8, 
        "published": 1413993669, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=tr1ca1ca1&url_id=Imh0dHA6Ly93d3cuZ3EuY29tL2VudGVydGFpbm1lbnQvY2VsZWJyaXRpZXMvMjAxNDExL25pY2tpLW1pbmFqIg.uPEKXCAr1mB_iEFaZ2UdIDqLhcY&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=8", 
        "source": "http://digg.com/", 
        "title": "Nicki Minaj, Cheeky Genius", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=tr1ca1ca1&url_id=Imh0dHA6Ly93d3cuZ3EuY29tL2VudGVydGFpbm1lbnQvY2VsZWJyaXRpZXMvMjAxNDExL25pY2tpLW1pbmFqIg.uPEKXCAr1mB_iEFaZ2UdIDqLhcY&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=8"
      }, 
      {
        "body": "The trio of girls from suburban Denver suspected of trying to join Islamist militants in Syria appear to be impressionable teens lured by the promise of adventure abroad \u2014 not steely-eyed zealots intent on perpetrating violence, officials told NBC News.\n\nOfficials said federal authorities are unlikely to charge the girls \u2014 described by law enforcement as 15- and 17-year-old sisters and a 16-year-old from another family \u2014 because they're minors. The prosecution of juveniles in the federal system is rare and complicated. In this case, the ages of the girls is a \"complicating factor\" that will likely keep them out of the courtroom, said David Raskin, a former federal prosecutor.\n\nIn the unlikely event the girls are prosecuted, they could be charged with juvenile delinquency. But even then, they would be released at age 18, per Justice Department policy.\n\nThe unidentified teens were intercepted by American law enforcement authorities at Frankfurt Airport over the weekend and returned to their families in Denver, federal law enforcement officials said Tuesday. An official said the eldest girl, who is of Somali origin, came up with the idea to go to Syria and coaxed the two younger girls to tag along. It was not clear Wednesday whether the girls had an actual contact in Syria \u2014 or if they were simply planning on showing up in the tumultuous country to volunteer with ISIS or another terror group, officials said.\n\nGerman authorities said Tuesday that no investigation was opened there, because there was no indication of criminal or terrorist activity.\n\nClick here to explore interactive map with details of the cases of the dozen U.S. residents \u2014 11 of them Americans older than 18 \u2014 accused of trying to join the fight in Iraq or Syria, as well as the three Americans confirmed to have died in the fighting.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/9346263f77594ed599d6a70e39c2f98e_medium.png"
          }, 
          "original": {
            "size": [
              2500, 
              1484
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/9346263f77594ed599d6a70e39c2f98e.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/9346263f77594ed599d6a70e39c2f98e_thumb.png"
          }
        }, 
        "index": 9, 
        "published": 1413993065, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=84&sm=1&a_id=ve1ve1de1&url_id=.eJwVykEOwzAIBMC_5E5Qmp76m8TBKqoLEYtl-fdV5zzLO_N-MY8xVjuLycBa_MtIj9nUhBUKSonw4CoXqFvTj7RJdzik9BTCDD3o9G4Xdfp3MZDXqkWPBrLHvj33bfkBCzEolw.ahyazkwypaOcgwUjQG2v_yW466Y&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=9", 
        "source": "http://nbcnews.com/", 
        "title": "Charges Unlikely for Syria-Bound American Teens", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=84&a_id=ve1ve1de1&url_id=.eJwVykEOwzAIBMC_5E5Qmp76m8TBKqoLEYtl-fdV5zzLO_N-MY8xVjuLycBa_MtIj9nUhBUKSonw4CoXqFvTj7RJdzik9BTCDD3o9G4Xdfp3MZDXqkWPBrLHvj33bfkBCzEolw.ahyazkwypaOcgwUjQG2v_yW466Y&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=9"
      }, 
      {
        "body": "Federal health officials announced Wednesday that all travelers from West African countries affected by the Ebola outbreak will be monitored for 21 days upon entering the U.S., in a new program scheduled to start Monday.\nThe new measures, announced by Tom Frieden, the director of the Centers for Disease Control and Prevention (CDC), represent a significant escalation in the government's attempts to reduce the risk of additional Ebola cases in the U.S.\nAccording to Frieden, the level of \"active monitoring\" will depend on whether a traveler had close contact with an Ebola patient. Someone who had little to no interaction with Ebola patients would have to self-report body temperatures to local health authorities, while someone who had significant exposure to a sick person's bodily fluids would be fully quarantined.\n\u201cThere are a variety of situations and it would be individualized,\u201d Frieden said, speaking on a conference call with reporters. \u201cWe will require a quarantine for the highest risk group.\u201d\nThe new measures will be implemented by six states: New York, Pennsylvania, Maryland, Virginia, New Jersey and Georgia. Those states are the destinations of about 70% of all travelers from Liberia, Sierra Leone and New Guinea. It wasn't immediately clear how travelers to other states would be tracked.\nOn Tuesday, the government had already mandated that all travelers from the three countries fly to one of the five airports already screening for the disease, in New York, New Jersey, Chicago, Atlanta and Washington, D.C.\nThe new monitoring will cover visitors, aid workers, journalists, CDC employees and other Americans returning from Liberia, Sierra Leone or Guinea, and could be expanded if Ebola spreads to other countries.\nFrieden said state and local health officials would check daily for fever or other Ebola symptoms. Passengers will get kits to help them track their temperature and will be told to inform health officials daily of their status. Check-ins could happen in person, via phone, Skype or FaceTime, or through employers.\nAnyone who had close contact with Ebola patients in Africa would not be permitted to travel commercially via bus, rail, air or other means, until the end of the 21-day window, Frieden said. \u201cIf they have high risk and they are not sick, then they would need to be quarantined \u2026 and they would not be permitted to travel by commercial conveyance,\u201d he said.\nThe monitoring window is three weeks long because that is the longest known period of incubation for the deadly Ebola virus, which has sickened nearly 10,000 in Africa and killed nearly 5,000, according to the World Health Organization.\nFrieden said the new system will likely warn of more suspected cases of Ebola, since the start of flu season means that \"it is not rare for people to have symptoms that may be consistent\" with Ebola, such as a fever and headache.\nAs for when the monitoring program will end, Frieden says the U.S. cannot let its guard down until the outbreak in West Africa is over.\n\u201cThis measure has been in the works for a long time,\u201d Frieden said. \u201cThis is another step to protect families, communities and health care workers from Ebola.\u201d\nThree individuals have been diagnosed with Ebola in the U.S., including two nurses who treated the first patient, Thomas Eric Duncan, in Dallas. Since Duncan died on Oct. 8, the CDC has been scrambling to improve guidance to health care workers and assure the public that safeguards are in place to deal with additional travelers from West Africa who may be carrying the virus across the Atlantic.\nRejecting lawmakers' requests for a travel ban from West Africa, Frieden said that once this program begins, there will be checks for signs of Ebola at the point of exit, entry, and for 21 days after entry.\n\u201cWe can do a lot of things to reduce the risk \u2026 but until it is stopped at the source, we can\u2019t make the risk zero here.\u201d\nMashable is a leading source for news, information and resources for the Connected Generation. Mashable reports on the importance of digital innovation and how it empowers and inspires people around the world. Mashable's record 40 million unique visitors worldwide and 19 million social media followers are one of the most influential and engaged online communities. Founded in 2005, Mashable is headquartered in New York City with an office in San Francisco.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/966296149c20468fa6036946a9aff46d_medium.png"
          }, 
          "original": {
            "size": [
              1200, 
              627
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/966296149c20468fa6036946a9aff46d.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/966296149c20468fa6036946a9aff46d_thumb.png"
          }
        }, 
        "index": 10, 
        "published": 1413997625, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=86&sm=1&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9tYXNoYWJsZS5jb20vMjAxNC8xMC8yMi9lYm9sYS1jZGMtYWN0aXZlLW1vbml0b3JpbmcvIg.q9jDcTT7SrEWVp3a9gVNU4P613o&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=10", 
        "source": "http://mashable.com/", 
        "title": "U.S. Will Now Monitor All Travelers From Ebola Zone for 21 Days", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=86&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9tYXNoYWJsZS5jb20vMjAxNC8xMC8yMi9lYm9sYS1jZGMtYWN0aXZlLW1vbml0b3JpbmcvIg.q9jDcTT7SrEWVp3a9gVNU4P613o&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=10"
      }, 
      {
        "body": "In January 2013, strewn amid the rubble and debris left after a terrorist attack on a gas plant in the Algerian desert were the remains of two men who had traveled far from home to wage what they viewed as a holy war.\n\nThe men had been friends in high school in Ontario, Canada, before they set off on a journey in 2011 that would take them to Morocco, Mauritania, a terrorist training camp in Mali and, ultimately, to their deaths in the sands of Algeria.\n\nThe forces that drove the men, Xris Katsiroubas and Ali Medlej, from their sedate life in Canada have only gathered momentum since then, both in Canada and in other Western nations.\n\nIn recent months, more than 100 Canadians have sought out conflicts in foreign lands from Somalia to Syria, according to a government report.\n\nThe threat was brought home for Canadians first on Monday, when a man who was inspired by Islamic extremists based overseas used his car to run down and kill a soldier in Quebec. The man was later killed by the police.\n\nOn Wednesday, Ottawa, the country\u2019s capital, was locked down after a gunman shot and killed a soldier at a war memorial and then stormed the nation\u2019s Parliament building. The gunman, who himself was fatally shot, was identified by the authorities as a young man who had recently converted to Islam.\n\nPrime Minister Stephen Harper, who spoke to the nation from an undisclosed location on Wednesday evening, said that while the motive behind the attack that day was under investigation, the act had clearly been meant to terrorize. He said the attack was a \u201cgrim reminder\u201d of the threats that the country faces.\n\nLike other Western nations, Canada is struggling both to understand the phenomenon and to ensure that extremists who return home cause no harm.\n\nIts efforts took on added urgency after American-led airstrikes in Iraq and Syria against the extremist group called the Islamic State.\n\nMr. Harper has been a staunch defender of the effort to destroy the Islamic State, also known as ISIS. On Oct. 8, Canadian lawmakers voted to authorize the nation\u2019s military to participate in the strikes in Iraq.\n\n\u201cIf left unchecked, this terrorist organization will grow and grow quickly,\u201d Mr. Harper said when the measure passed. \u201cThey have already voiced their local and international terrorist intentions and identified Canada as a potential target.\u201d\n\nMr. Harper was referring to comments made by Abu Muhammad al-Adnani, an Islamic State spokesman, who sought to rally fighters to the group\u2019s cause and urged individual Muslims to attack civilians.\n\nMr. Adnani exhorted them to \u201ckill a disbelieving American or European \u2014 especially the spiteful and filthy French \u2014 or an Australian, or a Canadian, or any other disbeliever from the disbelievers waging war, including the citizens of the countries that entered into a coalition against the Islamic State.\u201d\n\nThe threat of a \u201clone wolf\u201d attack is a top concern for Western security agencies, including Canada\u2019s. \u201cTerrorism remains the leading threat to Canada\u2019s national security,\u201d wrote Steven Blaney, minister of public safety and emergency preparedness, in a September report on the terrorist threat to the country.\n\n\u201cAs of early 2014, the government was aware of more than 130 individuals with Canadian connections who were abroad and who were suspected of terrorism-related activities,\u201d the report said.\n\nWhile the idea that individuals are leaving their country of residence to take up arms in a foreign conflict is hardly new or unique to Canada, the report found that the number of people choosing to do so had picked up pace in recent months.\n\nThe report said Canadians had engaged in \u201ctraining, fund-raising, promoting radical views and even planning terrorist violence.\u201d\n\n\u201cSome extremist travelers remain abroad,\u201d the report said. \u201cOthers have returned to Canada, while still others are presumed dead.\u201d It said at least 30 \u201cindividuals with a Canadian connection\u201d were involved in terrorist-related activity in Syria.\n\nMichel Coulombe, the director of the Canadian Security Intelligence Service, told lawmakers this month that the authorities were also looking into the activities of 80 people who had been radicalized, had traveled overseas and had returned home.\n\nHe said the government knew who these individuals were and where they were.\n\nBut he also cautioned calm, saying there was no intelligence indicating an imminent attack.\n\nNearly two weeks later, a man in Quebec turned his car into a deadly weapon, running over and killing a warrant officer and injuring a soldier.\n\nIt soon emerged that the driver of the car, Martin Rouleau-Couture, had been under watch by the police and had his passport seized after he tried to fly to Turkey to join the Islamic State.\n\nHe was one of 90 people being monitored as a part of 63 active national security investigations, according to Bob Paulson, the commissioner for the Royal Canadian Mounted Police.\n\n\u201cHe was part of our investigative efforts to try and identify those people who might commit a criminal act of traveling abroad for terrorist purposes,\u201d Mr. Paulson said.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/d094923a3d5741589fd907ca12504f44_medium.png"
          }, 
          "original": {
            "size": [
              1050, 
              591
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/d094923a3d5741589fd907ca12504f44.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/d094923a3d5741589fd907ca12504f44_thumb.png"
          }
        }, 
        "index": 11, 
        "published": 1414032978, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=36&sm=1&a_id=ttmv1tv1so1&url_id=.eJwNyDEOgCAMAMC_uJeCOvmbCk0koWLaGvT3euNNh_u1IY4xwvl6FbaQu-Ac04op4rzg6NoKkrDWTIaZTioE_2plAzLgx5WlmkC79S_pykC7dirhcGnTB_hXJAc.u_hZ0b3_CiD7DY_lPlv4SrcJ_XU&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=11", 
        "source": "http://nytimes.com/", 
        "title": "Canada Worries as Extremism Lures More Abroad", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=36&a_id=ttmv1tv1so1&url_id=.eJwNyDEOgCAMAMC_uJeCOvmbCk0koWLaGvT3euNNh_u1IY4xwvl6FbaQu-Ac04op4rzg6NoKkrDWTIaZTioE_2plAzLgx5WlmkC79S_pykC7dirhcGnTB_hXJAc.u_hZ0b3_CiD7DY_lPlv4SrcJ_XU&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=11"
      }, 
      {
        "body": "As the NFL's trading deadline -- Tuesday, Oct. 28, at 4 p.m. ET -- approaches, we explore four explosive, albeit unlikely, possible deals.\n\nNew England Patriots quarterback Tom Brady to the Texans for Houston's 2015 first-round draft pick and wide receiver Andre Johnson\n\nBefore you scroll down to the comments section and leave the obligatory nasty note, consider that we asked a current NFL general manager if this incendiary, social media-exploding potential deal was plausible.\n\n\"Absolutely,\" he said. \"It actually makes too much sense. The players in the Patriots' locker room know that their days are numbered. That's just the way it is in New England.\"\n\nTom Brady, the unlikely sixth-round draft choice who delivered three Super Bowl victories in a span of four years, knows this better than anyone. It happened to Drew Bledsoe, a franchise quarterback who lost his job to Brady early in the 2001 season, watched him win a Super Bowl and then was shuffled off to Buffalo ... for a first-round draft choice.\n\n\"If you play for the Patriots -- and, honestly, it doesn't matter if you're Tom Brady -- you're there as long as you're useful,\" Bledsoe said this past January in a television feature about the Patriot Way. \"Tom will have his time, too. And he knows that.\"\n\nThat time, in our admittedly feverish minds, is now. Sure, the Patriots are probably on their way to an 11th division title in 12 years -- something that hasn't happened since the AFL-NFL merger -- but they haven't won a Super Bowl in nearly a decade. Three years ago, the Patriots spent a third-round pick on quarterback Ryan Mallett. He was not the Brady heir they imagined and wound up in Houston. There is a feeling within the New England organization that Jimmy Garoppolo, this year's second-round draft choice, might be that guy. He broke some of Tony Romo's most cherished records at Eastern Illinois, and, with Brady in what is widely perceived as decline, this transition could work.\n\nThe biggest factor in this trade is the Patriots' institutional arrogance, i.e., the belief head coach Bill Belichick has in his ability to do what's best for the team. Belichick's signature personnel moves feature the departure of a startling series of aging but still serviceable players: Bledsoe, Lawyer Milloy, Ty Law, Damien Woody, Richard Seymour, Mike Vrabel, Wes Welker and, just prior to this season, Logan Mankins.\n\nHis Houston counterpart, head coach Bill O'Brien, is a huge Brady fan, having served as his quarterbacks coach and offensive coordinator and witnessed Brady's past two Super Bowl appearances from the Patriots' sideline. Ryan Fitzpatrick was O'Brien's choice to run Houston's offense, but wouldn't the Texans much rather have Brady in the huddle, showing the kind of emotion they already have on the other side of the ball with J.J. Watt? The Texans, who won two games a year ago, feel like they're getting closer to serious contention. Jadeveon Clowney, this year's No. 1 overall pick, looks ready to come back and contribute. Brady, even if he's sometimes missing targets he used to hit, would be a big addition.\n\nThere's precedent, too. Even the great Joe Montana, whom Brady idolized while growing up in the Bay Area, was sent packing by the 49ers, along with a safety and a third-round pick, for Kansas City's first-rounder. The Patriots, of course, would rather have DeAndre Hopkins, a 22-year-old version of Johnson, but they'll likely be content with the receiver who is 11 years his senior. New England would hope Johnson can contribute like another 30-something pickup back in 2007: Randy Moss.\n\nHere are the salary mechanics of the deal: To trade Brady before June 1, the Patriots would carry $18 million in dead money in 2015, the money left on his signing bonus. Cutting Peyton Manning cost the Colts $10.6 million against the cap two years ago, so there is a precedent for a large number when the salary is replaced by a rookie contract. Brady's contract is interesting. His salaries for 2015-17 (a total of $24 million) become fully guaranteed if he's on the roster for the last game of the 2014 season. Hmm.\n\nAfter an embarrassing Week 4 loss to the Chiefs, there were rumors Brady was at odds with the coaching staff's offensive philosophy. Welcome to Houston, Tom.\n\n\"I see the logic, but based on the last few games, I think it's too early to get on the Jimmy Garoppolo bandwagon,\" former Redskins and Texans general manager Charley Casserly said. \"I think Brady can still play.\"\n\nWhich is precisely why O'Brien and the Texans have to scoop him up. Brady knows their system, and he gives them instant credibility. The Patriots get a desperately needed wide receiver and a valuable first-round pick in return.\n\nLast year, before he played the Broncos, Brady was asked in an ESPN interview how he was coping with the loss of Welker.\n\n\"I'm used to it at this point,\" Brady said. \"It's just the way it is. You have to be mentally tough enough to put those things aside and still perform at a high level. Because if you don't, there's going to be someone else here ready to take your job.\"", 
        "images": {
          "medium": {
            "size": [
              500, 
              347
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/68c832993e564a10968c2fcfafa3207c_medium.png"
          }, 
          "original": {
            "size": [
              576, 
              400
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/68c832993e564a10968c2fcfafa3207c.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/68c832993e564a10968c2fcfafa3207c_thumb.png"
          }
        }, 
        "index": 12, 
        "published": 1414001820, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=70&sm=1&a_id=tr1ca1ca1&url_id=.eJwVzDESgkAMQNG70IcIY0XpGeydwMZdxyWJ2TDK7YX-v9-VCJsQuZn0WftFV5RnxRbqOz7QKDMWDWdKw3W4jOP9dgYQTonBXE0bVRD-AkuuJAmMwl8aDT4bebDPtLwhdIX5MDsU3Y67QPCPpHV_4vAvtw.3-cuzek0_4U4MS0Z833P69F8bgI&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=12", 
        "source": "http://digg.com/", 
        "title": "Tom Brady To The Texans?", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=70&a_id=tr1ca1ca1&url_id=.eJwVzDESgkAMQNG70IcIY0XpGeydwMZdxyWJ2TDK7YX-v9-VCJsQuZn0WftFV5RnxRbqOz7QKDMWDWdKw3W4jOP9dgYQTonBXE0bVRD-AkuuJAmMwl8aDT4bebDPtLwhdIX5MDsU3Y67QPCPpHV_4vAvtw.3-cuzek0_4U4MS0Z833P69F8bgI&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=12"
      }, 
      {
        "body": "The Republicans want to overhaul scandal-plagued federal agencies in 2015, the majority leader says.\n\nHouse Republicans haven't officially locked down their majority for next year, but they're already sketching out a legislative agenda for when they do.\n\nIn a memo to lawmakers on Wednesday, Majority Leader Kevin McCarthy said the party would target the federal bureaucracy with an eye toward restoring \"competence\" across a range of scandal-plagued departments and agencies. He cited the well-documented problems at the Veterans Administration, the Secret Service, the IRS, last year's launch of the federal health insurance exchanges, and the more recent response to Ebola, along with several other missteps that haven't garnered as much attention.\n\n\"Every week seems to bring a new revelation of government agencies failing to accomplish their core functions,\" McCarthy wrote.\n\nRepublicans are widely expected to expand their hold on the House in November, and they seem likely to take the Senate as well. The agenda McCarthy laid out, however, is fairly modest in scope, and probably not exhaustive; there are no new promises to repeal Obamacare, gut the EPA, or overhaul entitlement programs. Those may still be on the way, particularly if Republicans succeed in winning control of the Senate.\n\nYet McCarthy's plan to focus on competency dovetails with the party's campaign-trail arguments that the Obama administration lacks basic management skills. It also comports with the GOP's broader goal of reducing the size of the federal bureaucracy.\n\n\"Inefficient, ineffective, and incompetent federal agencies along with failed government policies have real world consequences,\" McCarthy wrote.\n\n\"They hurt economic growth and job creation. Restoring economic growth and job creation will be the central policy goal of the next Congress and restoring competence in government will be part of that effort. The inability of the government to accomplish its most basic tasks has eroded the public\u2019s trust in government, as polls have repeatedly shown. Worse, throughout the country there is an emerging sense of resignation that our great country is on the decline. We must work to end this cycle of failings and make government functional again.\"\n\nFixing the nuts and bolts of government isn't sexy, but it does have the potential to gain bipartisan support. The test for McCarthy and Speaker John Boehner will be whether the Republican agenda leans more toward \"reform,\" which could gain Democratic votes, or toward \"cuts,\" which probably will not. McCarthy's memo was light on specifics, mentioning only a series of bills the House has previously passed along with an idea to cut down on the thousands of annual reports that agencies must file according to congressional statutes.\n\nFor House Republicans, a focus on \"competency\" is a political safe harbor: It's straightforward and hard to oppose. But dozens of conservatives are already anxious for the party to adopt a more ambitious agenda in coordination with a GOP majority in the Senate, which the polls show is increasingly likely. They're going to want to cut a lot more than some agency reports.", 
        "images": {
          "medium": {
            "size": [
              500, 
              337
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/be19cd63ce6f44e0afb32d68828d95d2_medium.png"
          }, 
          "original": {
            "size": [
              615, 
              415
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/be19cd63ce6f44e0afb32d68828d95d2.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/be19cd63ce6f44e0afb32d68828d95d2_thumb.png"
          }
        }, 
        "index": 13, 
        "published": 1414014532, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=92&sm=1&a_id=tt1to1da1&url_id=.eJwNy0EKhTAMRdG9OI-v9QuKuykl_BY0KTaa7dvZHZw7FbN2AO4-W-FkZxKrec56oelZR3ekO5f6MpYQV8SAAano05n-2joJO3m6SYWqjLGxsWTGb4972DB9EzIiug.k-Lw3_yWmNWlWWGz4WFPHCVn63w&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=13", 
        "source": "http://marcambinder.theatlantic.com/", 
        "title": "The House GOP's New War on Incompetence", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=92&a_id=tt1to1da1&url_id=.eJwNy0EKhTAMRdG9OI-v9QuKuykl_BY0KTaa7dvZHZw7FbN2AO4-W-FkZxKrec56oelZR3ekO5f6MpYQV8SAAano05n-2joJO3m6SYWqjLGxsWTGb4972DB9EzIiug.k-Lw3_yWmNWlWWGz4WFPHCVn63w&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=13"
      }, 
      {
        "body": "We\u2019ve never understood the vitriol between loyal followers of LeBron James and Kobe Bryant. Both players are not only unquestioned all-time greats, but also reigned supreme in the NBA at disparate times \u2013 Kobe\u2019s prime coincided with LeBron\u2019s slow maturation, and the latter\u2019s prime is currently coinciding with the former\u2019s slow descent. Appreciating the gifts of one doesn\u2019t mean you can\u2019t similarly appreciate the other; their collective fandom isn\u2019t mutually exclusive.\n\nWhat makes the ongoing, seemingly never-ending war between each legion of fans ever-vexing is the adulation James and Bryant have openly shown one another over the past few seasons. They shared a special bond as leaders of the 2012 Olympic Team, one that began fostering when they were teammates on the Redeem Team four years earlier. LeBron and Kobe consistently commend the other through the media, and haven\u2019t been shy to exhibit kinship on the court, either.\n\nRemember this awesome Christmas moment from last season?\n\nJames lavished more praise on his fellow legend before the Cleveland Cavaliers\u2019 exhibition game today against the Dallas Mavericks, expressing empathy for Bryant\u2019s unenviable situation with the Los Angeles Lakers and raving about his notorious competitiveness.\n\nWe speak from know-how: Liking both players lends a far more enjoyable NBA experience than irrationally hating one of them. And considering the friendship James and Bryant share, we think it\u2019s safe to say they\u2019d advise you to adopt that very mentality.\n\n", 
        "images": {}, 
        "index": 14, 
        "published": 1413588627, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=on1ca1ca1&url_id=.eJxTyigpKbDS10_JzE3NTUzXS87P1TcyMDTRNzTQz0lNKsrP083JL0vVzc5PSoWwgCoKUksySzKB7LzEktIiVPG8dH0lAOetHkA.vF0X8DtGFAiJkCO57-aTwT7PgPQ&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=14", 
        "source": "http://dimemag.com/", 
        "title": "LeBron: \u201cI Love Kobe. I Love His Competitive Nature. I Love Competing Against Him\u201d", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=on1ca1ca1&url_id=.eJxTyigpKbDS10_JzE3NTUzXS87P1TcyMDTRNzTQz0lNKsrP083JL0vVzc5PSoWwgCoKUksySzKB7LzEktIiVPG8dH0lAOetHkA.vF0X8DtGFAiJkCO57-aTwT7PgPQ&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=14"
      }, 
      {
        "body": "The suspect in the killing of a Canadian soldier at an Ottawa war memorial wanted to travel to Syria and had a passport application delayed over extremism concerns.\n\nMichael Zehaf-Bibeau, 32, who was shot dead shortly after running into the Canadian parliament building, was not among 90 high-risk travellers being monitored by authorities, but was seeking a passport, police said in a news conference.\n\nHis mother told police he wanted to travel to Syria.\n\nPolice were asked to carry out background checks when he applied for the passport, but he had not been placed under surveillance.\n\nZehaf-Bibeau was Canadian, but may have also had dual Libyan citizenship, the news conference was told.\n\nOn Wednesday, he shot and killed a Canadian soldier at the Ottawa war memorial, before attempting to storm the parliament building, triggered a lockdown in the capital city.\n\nThe news conference heard that he had acted alone and police have not linked his attack with the killing of another soldier in Quebec on Monday.\n\nDelays in his passport application may have formed part of his motivation for the attack in Ottawa, according to police.\n\nBob Paulson, commissioner of the Royal Canadian Mounted Police (RCMP), said: \"We have no information linking the two attacks this week.\n\n\"The passport was part of his motivation. His application was not rejected. His passport was not revoked.\n\n\"He was waiting to get it and there was an investigating going on to determine to see whether he would get a passport.\"\n\nAn email from Zehaf-Bibeau was found on the hard drive of someone who has been charged with a terrorism-related offence in Canada, the RCMP said.\n\nOfficers said there were now 93 high-risk Canadians who have demonstrated an intention to travel abroad for militant reasons, but they had no plans to make any arrests at this time.\n\nZehaf-Bibeau was shot and killed by Sergeant-at-Arms Kevin Vickers, who was given a standing ovation during a special session of parliament on Thursday.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/1f0dfa3bfaef4fdaa055b475d7f73062_medium.png"
          }, 
          "original": {
            "size": [
              1600, 
              900
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/1f0dfa3bfaef4fdaa055b475d7f73062.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/1f0dfa3bfaef4fdaa055b475d7f73062_thumb.png"
          }
        }, 
        "index": 15, 
        "published": 1414099736, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=84&sm=1&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9uZXdzLnNreS5jb20vc3RvcnkvMTM1OTIwOC9jYW5hZGlhbi1ndW5tYW4td2FudGVkLXRvLXRyYXZlbC10by1zeXJpYSI.8McmLhPrjWi_ISDhbIdOxSwfGK0&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=15", 
        "source": "http://news.sky.com/", 
        "title": "Canadian Gunman Wanted To Travel To Syria", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=84&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9uZXdzLnNreS5jb20vc3RvcnkvMTM1OTIwOC9jYW5hZGlhbi1ndW5tYW4td2FudGVkLXRvLXRyYXZlbC10by1zeXJpYSI.8McmLhPrjWi_ISDhbIdOxSwfGK0&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=15"
      }, 
      {
        "body": "A hundred firemen could not prevent wooden cooling towers at Didcot B gas-fuelled power station in Oxfordshire from burning down. A consortium said it could power 2.5 million houses in Britain by 2018 with solar energy generated in southern Tunisia. The Bank of England indicated that interest rates would stay low for longer because of a poor outlook for the global economy. Government borrowing rose to \u00a311.8 billion in September: \u00a31.6 billion more than a year earlier. HSBC offered a mortgage at 0.99 per cent interest. The government is to pay a bounty of \u00a355 to GPs for every patient they diagnose with dementia. English hospitals near the Welsh border are under \u2018absolutely intolerable pressure\u2019 from patients crossing over to get treatment, Jeremy Hunt, the Health Secretary, said. The Duchess of Cambridge is expecting her second child next April.\n\nDavid Cameron said that before Christmas he would set out further plans to curb the rights of EU migrants to work in Britain. Not enough of the 10,650 foreign prisoners in Britain are being deported, according to the National Audit Office. Among those to be created peers were Sir Andrew Green, head of Migration Watch, and Sir Robert Rogers, the former Clerk of the House of Commons. A flock of sheep at Merstham, Surrey, devoured \u00a34,000-worth of cannabis that had been dumped in their field.\n\nBritain will fly unmanned drones over Syria. The Royal Fleet Auxiliary vessel Argus continued its passage to Sierra Leone to support action against Ebola; the hospital on board will not be used for Ebola patients. A man from Turvey, Bedfordshire, withdrew his daughter from school because it would not let her wear a face mask against Ebola. Tens of thousands of people in London, Glasgow and Belfast demonstrated in favour of higher pay, adopting the TUC slogan: \u2018Britain Needs a Pay Rise\u2019. A.H. Halsey, Britain\u2019s first professor of sociology and the scourge of grammar schools, died, aged 91. The 11th Duke of Marlborough died, aged 88. Raphael Ravenscroft, who played the saxophone solo on Gerry Rafferty\u2019s \u2018Baker Street\u2019, died, aged 60.\n\nSenegal and Nigeria were declared free of Ebola, which has killed more than 4,500, mostly in Liberia, Guinea, and Sierra Leone. The United States limited ingress to five airports for people from the worst affected countries. The Pentagon set up a 30-man rapid reaction medical support team to help with any cases of Ebola in the United States. The American government was found to have paid dozens of suspected Nazi war criminals millions of dollars in social security after they renounced their citizenship and agreed to leave the country. America\u2019s secret unmanned orbital test vehicle landed in California after 674 days in orbit.\n\nTurkey decided to allow Iraqi Kurdish fighters to cross the Syrian border to fight Islamic State troops in Kobane, where their assault had been driven back. American military aircraft dropped weapons and medical supplies to Kurdish forces there. An Islamic State video showed that what it said were American arms dropped in Syria had come into its hands.An Australian teenager appeared in an Islamic State video defying the prime minister of Australia. Gough Whitlam, prime minister of Australia from 1972 to 1975, when he was removed from office by the governor general, died, aged 98. Boko Haram killed people in three villages in north-east Nigeria, despite the government announcing a truce intended to secure the freedom of 200 abducted schoolgirls.\n\nA synod of bishops in Rome declared that \u2018homosexuals have gifts and qualities to offer to the Christian community\u2019 but said \u2018unions between people of the same sex cannot be considered on the same level as marriage between man and woman\u2019. Oscar Pistorius, the South African athlete, was sentenced to five years in jail for the culpable homicide of his girlfriend Reeva Steenkamp. President Vladimir Putin of Russia paid a visit to Silvio Berlusconi, the disgraced Italian former prime minister, in the small hours during the Asia-Europe summit in Milan. Christophe de Margerie, the chief executive of Total, and three crew died when his plane collided at Vnukovo airport with a snow plough. At least 41 trekkers were killed by snow storms in the Nepalese Himalayas.   CSH\n\nThis article first appeared in the print edition of The Spectator magazine, dated 25 October 2014", 
        "images": {
          "medium": {
            "size": [
              500, 
              333
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141222/66f10f79624e4e07a539258ecaff2a5e_medium.png"
          }, 
          "original": {
            "size": [
              620, 
              413
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141222/66f10f79624e4e07a539258ecaff2a5e.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141222/66f10f79624e4e07a539258ecaff2a5e_thumb.png"
          }
        }, 
        "index": 16, 
        "published": 1414033200, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=73&sm=1&a_id=tt1to1da1&url_id=Imh0dHA6Ly9zcGVjYy5pZS8xemxoUTROIg.n3iSWWuqMa1Ocp1CQtFg4uaeLl0&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=16", 
        "source": "http://www.spectator.co.uk/", 
        "title": "25 October 2014", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=73&a_id=tt1to1da1&url_id=Imh0dHA6Ly9zcGVjYy5pZS8xemxoUTROIg.n3iSWWuqMa1Ocp1CQtFg4uaeLl0&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=16"
      }, 
      {
        "body": "FACTS!\n\u2026They\u2019re a thing. We love them. We also know they\u2019re hard to come by on the Internet. That\u2019s why we have a team of fact-checkers double-checking everything we post, with standards that meet or exceed anyone else on the web. So go ahead and share your favorite thing from Upworthy with the full confidence that it's on the level \u2014 and that you\u2019ll look really smart doing it. Not that you need any help with that, of course.\nIf we discover that something less-than-facty slipped through the cracks, we\u2019ll always be up front with you. Check our corrections page for more information.\nCoke and Pepsi are spending millions of dollars to keep taxes from going up on their sugared products. Surprised? It's all thanks to the infamous Citizens United decision. Watch Robert Reich break it down.\nAbout\nJoin Us\nLegalese", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/db28c246dfaf4181ae023593bf60dea7_medium.png"
          }, 
          "original": {
            "size": [
              1200, 
              626
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/db28c246dfaf4181ae023593bf60dea7.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/db28c246dfaf4181ae023593bf60dea7_thumb.png"
          }
        }, 
        "index": 17, 
        "published": 1414000588, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=67&sm=1&a_id=tr1ca1ca1&url_id=.eJwdyksOgCAMBcC7uH-w9zYEKyWKJbWk4fZ-NrOahc36GqO7h9Fd1HiGLC2e9SBkeRFFp35XTBlotbDhEsMfjKkh3WgjM9JupP9iSgrnZF-YStikXmV5ALB6KHc.NStOXyMA_cF_r3TwjNYUx52RYas&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=17", 
        "source": "http://www.upworthy.com", 
        "title": "Like Coke Or Pepsi? You Might Not Like Them As Much After You Hear What They're Doing.", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=67&a_id=tr1ca1ca1&url_id=.eJwdyksOgCAMBcC7uH-w9zYEKyWKJbWk4fZ-NrOahc36GqO7h9Fd1HiGLC2e9SBkeRFFp35XTBlotbDhEsMfjKkh3WgjM9JupP9iSgrnZF-YStikXmV5ALB6KHc.NStOXyMA_cF_r3TwjNYUx52RYas&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=17"
      }, 
      {
        "body": "On Friday, Nigeria's government announced it had reached a deal with Boko Haram to release the approximately 200 schoolgirls held captive by the Islamist terror group since April.\n\nThe agreement, announced by the country's defense minister, also involves a cease fire between Boko Haram and Nigeria's military. The government expects the terror group will not back out on the deal. \"Commitment among parts of Boko Haram and the military does appear to be genuine,\" an official with Nigeria's security forces told Reuters Friday. \"It is worth taking seriously.\"\n\nBoko Haram militants abducted more than 300 schoolgirls from Chibok boarding school in northern Nigeria in mid-April, sparking a worldwide outcry and propelling the group onto to the international stage for the first time. Over fifty of the girls escaped early on. The rest have remained in captivity ever since.\n\nBoko Haram, whose name roughly means \"Western education is sinful,\" has been terrorizing Nigeria since 2009 in an effort to return the country to the pre-colonial era of Muslim rule. Over the past half-decade, the Islamist group has killed approximately 5,000 Nigerians the group regards as pro-government in attacks on schools, churches, and mosques, as well as military checkpoints, police stations, highways, and a bus station in the capital city of Abuja.", 
        "images": {
          "medium": {
            "size": [
              500, 
              280
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141216/d04623effe1645fdba11ecc41f6da94d_medium.png"
          }, 
          "original": {
            "size": [
              630, 
              354
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141216/d04623effe1645fdba11ecc41f6da94d.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141216/d04623effe1645fdba11ecc41f6da94d_thumb.png"
          }
        }, 
        "index": 18, 
        "published": 1413563087, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=on1ca1ca1&url_id=.eJwFwUEOhSAMBcC7uK9V4-rfpl9fAKUtKSRc35klj9F-zHPOVX1kxOOGvl6urP44H9t-8r6xlYQoYtSv7F5TidrpLbdJa7jp769TlhClQIV0kKQAFDaWDzzJJOU.Ewv2LcMdChoNz5_uJShYVmj6w8M&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=18", 
        "source": "http://motherjones.com/", 
        "title": "Finally, Nigeria's Kidnapped Schoolgirls Are Coming Home", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=on1ca1ca1&url_id=.eJwFwUEOhSAMBcC7uK9V4-rfpl9fAKUtKSRc35klj9F-zHPOVX1kxOOGvl6urP44H9t-8r6xlYQoYtSv7F5TidrpLbdJa7jp769TlhClQIV0kKQAFDaWDzzJJOU.Ewv2LcMdChoNz5_uJShYVmj6w8M&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=18"
      }, 
      {
        "body": "The teenage sisters told their father they were staying home sick from their suburban Denver school. Instead, they took $2,000 and their passports and headed off for Syria with a 16-year-old friend. They made it as far as Germany before border guards detained them for questioning.\n\nThe fact that adolescent girls could make their way across the Atlantic might come as a surprise to many parents, but a patchwork of laws and rules governing international air travel in many cases makes it easy for teenagers to travel with nobody's permission but their own.\n\nAirlines have a range of rules governing minors' travel: Many major carriers including United Airlines and Scandinavian airline SAS place no restrictions on children over 12, while others let even young minors travel as long as they are accompanied by someone over 16. Yet others, including American Airlines, require a parent to accompany travelers under the age of 15 to the gate, while those 15 and over face no restrictions.\n\nCountries have a separate set of laws that is no less haphazard, from a Russian requirement for notarized parental permission to the U.S. system where adolescents with valid passports are free to come and go.\n\nIn Spain, both parents must fill out a permission form at a police station before a minor can travel alone. In Germany, where the American teens were stopped, border guards are required to verify that minors have parental permission to travel.\n\nAnd in France, which is Europe's single largest source of would-be jihadis, parental authorization had to be received by city hall \u2014 until January 2013.\n\nThat's when a small administrative change took effect suspending the requirement for parental approval. The government said it would streamline unnecessary bureaucracy and officials remarked that few runaways went abroad, and even fewer stayed there.\n\nFast-forward 22 months, and nearly every week new reports emerge of French adolescents leaving for Syria. Teenagers from France can travel within the European Union with a valid ID; outside the EU, they need only a passport.\n\nUnder French law, parents can have their children flagged if they fear they will leave the country to join extremists. But for many of those who have left, their families had no warning.\n\nLawyer Agnes Dufetel-Cordier represents a teenage boy from Toulouse who left in January to join the al-Qaida-linked al-Nusra Front, before coming back to his family to face criminal charges. She said the teen \u2014 now 16 \u2014 gave no sign he was about to bolt for Syria, and his departure came as a shock to his parents. He was not stopped at the airport in Marseille, nor on arrival in Turkey or crossing into Syria.\n\n\"If you reverse the regulation that lets them travel without their parents' permission, you will see right away that minors are no longer leaving,\" Dufetel-Cordier said. \"Today in France, in the case of most minors who go to Syria, the families have absolutely no idea ahead of time.\"\n\nAt age 17, Sahra Ali Mehenni went so far as to ask her mother to get her a passport, saying she wanted her paperwork in order before she reached adulthood. When she left for Syria on March 11, departing from the Marseille airport just as the teen boy did, she took her burgundy-bound passport and nobody stopped her before she boarded the flight to Istanbul.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/21a2bab067f64880bac33893f5be0833_medium.png"
          }, 
          "original": {
            "size": [
              992, 
              558
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/21a2bab067f64880bac33893f5be0833.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/21a2bab067f64880bac33893f5be0833_thumb.png"
          }
        }, 
        "index": 19, 
        "published": 1414055960, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=84&sm=1&a_id=ve1ve1de1&url_id=.eJwFwdsJgDAMAMBd_E8Dis8N_HaCWIIWbFKSgLi9d90d0TZEOrPw6-nSlLXiLsEmFEWFHnyL8RFqHwazQCP3phbgnxWCsNLAmerD7tBPwzrPy9j99ywgqg.Qs7MVeLZ0cmPW-cWeIR6RxcmCBg&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=19", 
        "source": "http://abcnews.go.com/", 
        "title": "For Teen With Passport, Syria Trip Can Be Seamless", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=84&a_id=ve1ve1de1&url_id=.eJwFwdsJgDAMAMBd_E8Dis8N_HaCWIIWbFKSgLi9d90d0TZEOrPw6-nSlLXiLsEmFEWFHnyL8RFqHwazQCP3phbgnxWCsNLAmerD7tBPwzrPy9j99ywgqg.Qs7MVeLZ0cmPW-cWeIR6RxcmCBg&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=19"
      }, 
      {
        "body": "The first case of Ebola has been reported in Mali. Mali shares a border with Guinea, where the current Ebola outbreak began, but it has not seen any cases until now.\n\n\"Health Minister Ousmane Kone told state television that the patient in the western region of Kayes was a two-year-old girl who had recently arrived from neighboring Guinea,\" Reuters reported. Siguiri, a mining town in the northeast corner of Guinea, is the only Guinean district that shares a border with Mali and has reported Ebola cases.\n\nHere's a look at the Ebola outbreak in West Africa, the largest in history, with an arrow pointing to Mali:\n\nThere have been thousands of cases in Guinea, Sierra Leone, and Liberia; 20 cases in Nigeria; and isolated cases in Senegal, the United States, and Spain.\n\nAccording to the latest report from the World Health Organization, there have been 9,936 cases and 4,877 deaths reported in this outbreak, although the actual numbers may be three times as high.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/a26207b0966e47d1b60d2ef62ceb49ce_medium.png"
          }, 
          "original": {
            "size": [
              2343, 
              1757
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/a26207b0966e47d1b60d2ef62ceb49ce.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/a26207b0966e47d1b60d2ef62ceb49ce_thumb.png"
          }
        }, 
        "index": 20, 
        "published": 1414099740, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=85&sm=1&a_id=ve1ve1de1&url_id=Imh0dHA6Ly93d3cuYnVzaW5lc3NpbnNpZGVyLmNvbS9lYm9sYS1oYXMtbm93LXNwcmVhZC10by1tYWxpLTIwMTQtMTAi.GxwZz-ZgbsIP20ob4lgm-NcNpqQ&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=20", 
        "source": "http://businessinsider.com/", 
        "title": "Ebola Has Now Spread To Mali", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=85&a_id=ve1ve1de1&url_id=Imh0dHA6Ly93d3cuYnVzaW5lc3NpbnNpZGVyLmNvbS9lYm9sYS1oYXMtbm93LXNwcmVhZC10by1tYWxpLTIwMTQtMTAi.GxwZz-ZgbsIP20ob4lgm-NcNpqQ&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=20"
      }, 
      {
        "body": "A federal jury in Washington, D.C., returned guilty verdicts against four Blackwater operatives charged with killing more than a dozen Iraqi civilians and wounding scores of others in Baghdad in 2007.\n\nThe jury found one guard, Nicholas Slatten, guilty of first-degree murder, while three other guards were found guilty of voluntary manslaughter: Paul Slough, Evan Liberty, and Dustin Heard. The jury is still deliberating on additional charges against the operatives, who faced a combined 33 counts, according to the Associated Press. A fifth Blackwater guard, Jeremy Ridgeway, had already pleaded guilty to lesser charges and cooperated with prosecutors in the case against his former colleagues. The trial lasted ten weeks and the jury has been in deliberations for 28 days.\n\nThe incident for which the men were tried was the single largest known massacre of Iraqi civilians at the hands of private U.S. security contractors. Known as \u201cBaghdad\u2019s bloody Sunday,\u201d operatives from Blackwater gunned down 17 Iraqi civilians at a crowded intersection at Nisour Square on September 16, 2007. The company, founded by secretive right-wing Christian supremacist Erik Prince, pictured above, had deep ties to the Bush Administration and served as a sort of neoconservative Praetorian Guard for a borderless war launched in the immediate aftermath of 9/11.\n\nWhile Barack Obama pledged to reign in mercenary forces when he was a senator, once he became president he continued to employ a massive shadow army of private contractors. Blackwater \u2014 despite numerous scandals, congressional investigations, FBI probes and documented killings of civilians in both Iraq and Afghanistan \u2014 remained a central part of the Obama administration\u2019s global war machine throughout his first term in office.\n\nJust as with the systematic torture at Abu Ghraib, it is only the low level foot-soldiers of Blackwater that are being held accountable. Prince and other top Blackwater executives continue to reap profits from the mercenary and private intelligence industries. Prince now has a new company, Frontier Services Group, which he founded with substantial investment from Chinese enterprises and which focuses on opportunities in Africa. Prince recently suggested that his forces at Blackwater could have confronted Ebola and ISIS. \u201cIf the administration cannot rally the political nerve or funding to send adequate active duty ground forces to answer the call, let the private sector finish the job,\u201d he wrote.\n\nNone of the U.S. officials from the Bush and Obama administrations who unleashed Blackwater and other mercenary forces across the globe are being forced to answer for their role in creating the conditions for the Nisour Square shootings and other deadly incidents involving private contractors. Just as the main architect of the CIA interrogation program, Jose Rodriguez, is on a book tour for his propagandistic love letter to torture, Hard Measures: How Aggressive CIA Actions After 9/11 Saved American Lives, so too is Erik Prince pushing his own revisionist memoir, Civilian Warriors: The Inside Story of Blackwater and the Unsung Heroes of the War on Terror.\n\nWhile the Blackwater verdict is an important and rare moment of accountability in an overwhelmingly unaccountable private war industry, it does not erase the fact that those in power\u2014the CEOs, the senior officials, the war profiteers\u2014walk freely and will likely do so for the rest of their lives.\n\nWhat is so seldom discussed in public discourse on the use of mercenaries are the stories of their victims. After the Nisour Square massacre, I met with Mohammed Kinani, whose 9-year-old son, Ali, was the youngest person killed by Blackwater operatives that day. As he and his family approached the square in their car:\n\n\u201c[T]hey saw one armored vehicle and then another, with men brandishing machine guns atop each one,\u201d Mohammed recalls. The armored cars swiftly blocked off traffic. One of the gunners held both fists in the air, which Mohammed took as a gesture to stop. \u201cMyself and all the cars before and behind me stopped,\u201d Mohammed says. \u201cWe followed their orders. I thought they were some sort of unit belonging to the American military, or maybe just a military police unit. Any authority giving you an order to stop, you follow the order.\u201d It turns out the men in the armored cars were neither U.S. military nor MPs. They were members of a Blackwater team code-named Raven 23. As the family waited in traffic, two more Blackwater vehicles became visible. Mohammed noticed a family in a car next to his\u2014a man, woman and child. The man was staring at Mohammed\u2019s car, and Mohammed thought the man was eyeing Jenan. \u201cI thought he was checking my sister out,\u201d Mohammed remembers. \u201cSo I yelled at him and said, \u2018What are you looking at?\u2019\u201d Mohammed noticed that the man looked frightened. \u201cI think they shot the driver in the car in front of you,\u201d the man told him. Mohammed scanned the area and noticed that the back windshield of the white Kia sedan in front of him was shattered. The man in the car next to Mohammed began to panic and tried to turn his car around. He ended up bumping into a taxi, and an argument ensued. The taxi driver exited his car and began yelling. Mohammed tried to break up the argument, telling the taxi driver that a man had been shot and that he should back up so the other car could exit. The taxi driver refused and got back into his vehicle. At that point, an Iraqi police officer, Ali Khalaf Salman, approached the Kia sedan, and it started to slowly drift. The driver had been shot, and the car was gliding in neutral toward a Blackwater armored car. Salman, in an interview, described how he tried to stop it by pushing backward. He saw a panicked woman inside the car; she was clutching a young man covered in blood who had been shot in the head. She was shrieking, \u201cMy son! My son! Help me, help me!\u201d Salman remembered looking toward the Blackwater shooters. \u201cI raised my left arm high in the air to try to signal to the convoy to stop the shooting.\u201d He said he thought the men would cease fire, given that he was a clearly identified police officer. \u201cAs the officer was waving, the men on the armored cars started shooting at that car,\u201d Mohammed says. \u201cAnd it wasn\u2019t warning shots; they were shooting as in a battle. It was as though they were in a fighting field. I thought the police officer was killed. It was insane.\u201d Officer Salman managed to dive out of the way as the bullets rained down. \u201cI saw parts of the woman\u2019s head flying in front of me,\u201d recalled his colleague, Officer Sarhan Thiab. \u201cThey immediately opened heavy fire at us.\u201d \u201cWhat can I tell you?\u201d Mohammed says, closing his eyes. \u201cIt was like the end of days.\u201d Mohammed would later learn that the first victims that day, in the white Kia, were a young Iraqi medical student, Ahmed Haithem Al Rubia\u2019y, and his mother, Mahassin, a physician. Mohammed is crystal clear that the car posed no threat. \u201cThere was absolutely no shooting at the Blackwater men,\u201d he says. \u201cAll of a sudden, they started shooting in all directions, and they shot at everyone in front of them. There was nothing left in that street that wasn\u2019t shot: the ground, cars, poles, sidewalks; they shot everything in front of them.\u201d As the Blackwater gunners shot up the Rubia\u2019ys\u2019 vehicle, Mohammed said, it soon looked like a sieve \u201cdue to how many bullet holes it had.\u201d A Blackwater shooter later admitted that they also fired a grenade at the car, causing the car to explode. Mohammed says the Blackwater men then started firing across the square. \u201cThey were shooting in all directions,\u201d he remembers. He describes the shooting as \u201crandom yet still concentrated. It was concentrated and focused on what they aimed at and still random as they shot in all directions.\u201d One of the Blackwater shooters was on top of an armored vehicle firing an automatic weapon, he says. \u201cEvery time he would finish his clip, he would throw it on the ground and would load another one in and would start shooting again, and finish the new one and replace it with another.\u201d One young Iraqi man got out of his car to run, and as he fled, the Blackwater shooter gunned him down and continued firing into his body as it lay on the pavement, Mohammed says. \u201cHe was on the ground bleeding, and they\u2019re shooting nonstop, and it wasn\u2019t single bullets.\u201d The Blackwater shooter, he says, would fire at other Iraqis and cars and then return to pump more bullets into the dead man on the ground. \u201cHe sank in his own blood, and every minute the [Blackwater shooter] would shoot left and right and then go back to shoot the dead man, and I could see that his body would shake with every bullet. He was already dead, but his body was still reacting to the bullets. [The shooter] would fire at someone else and then go back to shoot at this dead man.\u201d Shaking his head slowly, Mohammed says somberly, \u201cThe guy is dead in a pool of blood. Why would you continue shooting him?\u201d In his vehicle, as the shooting intensified, Mohammed yelled for the kids to get down. He and his sister did the same. \u201cMy car was hit many times in different places. All I could hear from my car was the gun shots and the sound of glass shattering,\u201d he remembers. Jenan was frantic. \u201cWhy are they shooting at us?\u201d she asked him. Just then, a bullet pierced the windshield, hitting Jenan\u2019s headrest. Mohammed shows me a photo of the bullet hole. As gunfire rained on the SUV, Jenan grabbed Mohammed\u2019s hair, yanked his head down and covered him with her body. \u201cMy young sister was trying to protect me by covering me with her body, so I forced myself out of her grip and covered her with my body to protect her. It was so horrific that my little sister, whom I\u2019m supposed to protect, was trying to protect me.\u201d Mohammed managed to slip his cellphone from his pocket and was going to call his father. \u201cIt\u2019s customary that when in agony before death, you ask those close to you to look after your loved ones,\u201d he says. Jenan demand", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/07a42b7afbef438ca455d1c03214fa40_medium.png"
          }, 
          "original": {
            "size": [
              1000, 
              710
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/07a42b7afbef438ca455d1c03214fa40.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/07a42b7afbef438ca455d1c03214fa40_thumb.png"
          }
        }, 
        "index": 21, 
        "published": 1414001820, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=64&sm=1&a_id=tr1ca1ca1&url_id=Imh0dHBzOi8vZmlyc3Rsb29rLm9yZy90aGVpbnRlcmNlcHQvMjAxNC8xMC8yMi9ibGFja3dhdGVyLWd1aWx0eS12ZXJkaWN0cy8i.EsSmmGP0833yvSaCWb60mnCZ_rw&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=21", 
        "source": "http://digg.com/", 
        "title": "Blackwater Founder Remains Free And Rich While His Former Employees Go Down On Murder Charges", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=64&a_id=tr1ca1ca1&url_id=Imh0dHBzOi8vZmlyc3Rsb29rLm9yZy90aGVpbnRlcmNlcHQvMjAxNC8xMC8yMi9ibGFja3dhdGVyLWd1aWx0eS12ZXJkaWN0cy8i.EsSmmGP0833yvSaCWb60mnCZ_rw&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=21"
      }, 
      {
        "body": "Good morning! Here's what you need to know for Thursday.\n\n1. Much of downtown Ottawa was on lockdown on Wednesday after a gunman, identified as Canadian Michael Zehaf-Bibeau, shot and killed a soldier at the National War Memorial on Parliament Hill.\n\n2. Russian prosecutors have detained four Moscow airport workers, which officials say might be responsible for the plane crash that killed the CEO of French oil giant Total, 63-year-old Christophe de Margerie.\n\n3. The World Health Organization updated its Ebola figures, warning that the virus could infect 10,000 people in West Africa by early December, while a total of 4,877 people have died from Ebola so far.\n\n4. The National Institutes of Health has begun early human testing of an Ebola vaccine, called VSV-ZEBOV.\n\n5. Tesco, the world's second-largest retailer, confirmed on Thursday that its first half pre-tax profit had been overstated by \u00a3263 million and announced that chairman Sir Richard Broadbent would step down.\n\n6. US-led airstrikes against Islamic State militants in Syria have killed 553 people over the last month, with most of the dead being members of the terrorist group.\n\n7. Swedish forces are still hunting for what it believes are mysterious foreign vessels illegally operating in its waters.\n\n8. Britain's National Health System says it needs an extra \u00a38 billion a year after warning of a \u00a330 billion annual shortfall that would develop by 2020.\n\n9. Apple said the company will open 25 stores in China within the next two years.\n\n10. Scientists have unraveled the oldest DNA ever, which comes from the femur of a man who died around 45,000 years ago.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/dcd38887b0524288b87a6986660c7629_medium.png"
          }, 
          "original": {
            "size": [
              2040, 
              1530
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/dcd38887b0524288b87a6986660c7629.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/dcd38887b0524288b87a6986660c7629_thumb.png"
          }
        }, 
        "index": 22, 
        "published": 1414036740, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=86&sm=1&a_id=tt1to1da1&url_id=.eJwlxkEKhDAMBdC7uP-2VVfeZtTSBmwiSYZcf4TZPN7U3Z89pYiYj68RV3sxuqrOp4xUMoaYg8Yj6h92eCduBuJ3FSF6X1Bq3cESkNPlqIplxZLL9qfk6QfbTSPy.lR2mtGVwn-_RTW56WByxQNyNVao&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=22", 
        "source": "http://businessinsider.com/clusterstock", 
        "title": "The 10 Most Important Things In The World Right Now", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=86&a_id=tt1to1da1&url_id=.eJwlxkEKhDAMBdC7uP-2VVfeZtTSBmwiSYZcf4TZPN7U3Z89pYiYj68RV3sxuqrOp4xUMoaYg8Yj6h92eCduBuJ3FSF6X1Bq3cESkNPlqIplxZLL9qfk6QfbTSPy.lR2mtGVwn-_RTW56WByxQNyNVao&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=22"
      }, 
      {
        "body": "A British man pleaded guilty this week to stealing 40,000 pounds from an elderly neighbor and pretending to be in a coma for two years to avoid charges, authorities said.\n\nAlan Knight pleaded guilty after being charged with multiple counts of theft and making a false representation for gain, a Swansea Crown Court representative told ABC News. He is scheduled to be sentenced on Nov. 7.\n\nKnight was arrested in 2012 for the alleged theft, a South Wales Police spokesman said.\n\nBut Knight delayed going to court by claiming to be a quadriplegic who had periodic seizures that left him in a comatose-state, police said. Since authorities were unable to get Knight in court, his trial was delayed until this week, police said.\n\nHowever, an investigation revealed that Knight had been faking his symptoms, police said.\n\nKnight and his wife, Helen Knight, even attempted to prove Knight's medical condition by photographing themselves in their home with Knight appearing to be unconscious and surrounded by medical equipment.\n\nHowever, earlier this week Knight was finally ordered to attend court in person. Once in the courtroom investigators revealed they had footage of Knight walking around on closed-circuit television without a neck brace, oxygen or a wheelchair, police said.\n\nIn images and video released to the news media, Knight is shown walking through a doorway with his family. After the evidence was presented, Knight then pleaded guilty to the charges.\n\nCalls to a number listed in the name of Knight\u2019s wife, Helen Knight, were not immediately returned.\n\nJudge Paul Thomas, who was overseeing Knight's case, said Knight's injury claim was \"unique\" and wanted to discourage anyone else who might try it, according to the Daily Telegraph.\n\n\"Although a very accomplished and determined actor, he is in nothing like the condition he claims to be, and the conditions he claims to be suffering from are simply non-existent,\" Thomas said in court, according to the Daily Telegraph.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/3703ec4b8d0f449b9d07516ac95a71b1_medium.png"
          }, 
          "original": {
            "size": [
              992, 
              558
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/3703ec4b8d0f449b9d07516ac95a71b1.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/3703ec4b8d0f449b9d07516ac95a71b1_thumb.png"
          }
        }, 
        "index": 23, 
        "published": 1413990812, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=on1ca1ca1&url_id=Imh0dHA6Ly9hYmNuZXdzLmdvLmNvbS9IZWFsdGgvYnJpdGlzaC1tYW4tZmFrZWQtY29tYS1hdm9pZC1jb3VydC1jb3BzL3N0b3J5P2lkPTI2Mzc5NzI5Ig.YAZ6BYT-TDpPLr48DrGh6oCAHXM&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=23", 
        "source": "http://abcnews.go.com/", 
        "title": "Man Faked Coma to Avoid Court, Cops Say", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=on1ca1ca1&url_id=Imh0dHA6Ly9hYmNuZXdzLmdvLmNvbS9IZWFsdGgvYnJpdGlzaC1tYW4tZmFrZWQtY29tYS1hdm9pZC1jb3VydC1jb3BzL3N0b3J5P2lkPTI2Mzc5NzI5Ig.YAZ6BYT-TDpPLr48DrGh6oCAHXM&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=23"
      }, 
      {
        "body": "Mursitpinar (Turkey) (AFP) - US-led air strikes in Syria were reported Thursday to have killed more than 500 jihadists in a month, as fighting raged in the embattled border town of Kobane.\n\nAn AFP correspondent across the frontier in Turkey reported fierce clashes in several parts of Kobane early Thursday, with heavy gun and mortar fire.\n\nThe town's Kurdish defenders have been holding out against an assault by the Islamic State militant group for more than a month, buoyed in recent days by a promise of Iraqi Kurd reinforcements and US air drops of weapons.\n\nFighter jets were again heard flying over Kobane on Thursday, the AFP reporter said, a month after the US-led coalition expanded its aerial campaign against IS in Iraq to Syria.\n\nThe air strikes have killed 553 people since their launch, the Syrian Observatory for Human Rights said, including 464 IS fighters and 57 militants from Al-Qaeda affiliate al-Nusra Front.\n\nThirty-two civilians have also been killed, including six children and five women, said the Britain-based Observatory, which relies on a wide network of sources inside Syria.\n\nObservatory director Rami Abdel Rahman told AFP that the \"vast majority\" of jihadists killed in the strikes were not Syrians but foreign fighters who had joined IS and Nusra in the country.\n\nAfter first focusing on Iraq, the coalition has dramatically expanded its strikes in Syria in recent days, including at Kobane which has become a crucial battleground in the fight against IS.\n\nThe jihadist group launched an offensive against the town last month, as it seeks to expand its control over large parts of Syria and Iraq where IS declared an Islamic \"caliphate\" earlier this year.\n\nAfter initially losing ground, the Kobane Kurds have fought back hard, with the US military saying they had halted the IS advance and held most of the town.\n\nBut local officials say the exhausted fighters are in desperate need of relief and anxious for promised reinforcements from Iraq's autonomous Kurdish region.\n\nIraqi Kurdish lawmakers in their capital Arbil agreed on Wednesday to send their peshmerga fighters, after Turkey this week said it would allow them to travel to Kobane.\n\nMustafa Qader, responsible for the peshmerga, said a decision would be made in the coming days about how many to send.\n\nHe did not say when the forces would arrive in Syria, but added that \"they will remain there until they are no longer needed\".\n\nIn Iraq, IS fighters had again surrounded Mount Sinjar in the country's north where they had trapped thousands of civilians this summer, commanders in the area said.\n\nThe civilians, mostly members of the Yazidi religious minority, eventually escaped via Syria with the help of Kurdish fighters from Iraq's neighbour to the west, but that route has now been cut.\n\n\"The mountain is besieged\" again, and IS militants are \"trying to climb the mountain on foot to fight the Yazidi volunteers,\" Dawud Jundi, a commander of the forces defending the area, told AFP by telephone.\n\nThe IS push began Monday, when some 300 of the militants with armoured vehicles attacked and seized nearby villages and then turned their attention on the mountain itself.\n\n\"We don't have anything but light weapons,\" Jundi said.\n\nOn Mount Sinjar, \"there are almost 2,000 families whose situations are very bad,\" he said.\n\nThe first siege of Mount Sinjar was a key moment in the conflict with IS, with the plight of the people trapped on the mountain helping to prompt Washington to begin air strikes against the jihadists.\n\nThe Iraqi capital Baghdad has also seen a wave of bomb attacks against Shiite targets in recent days, with IS claiming responsibility for some.\n\nAt least 28 people were killed on Wednesday when car bombs went off near a maternity hospital and a service station in areas of the capital where Shiites have frequently been targeted.\n\nThe bloodshed has raised fears of further attacks during the Ashura religious ritual in early November, when hundreds of thousands of Shiite faithful converge on the holy city of Karbala on foot.", 
        "images": {
          "medium": {
            "size": [
              500, 
              333
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/a252e3f96dc54efc952eb9e433b6f924_medium.png"
          }, 
          "original": {
            "size": [
              600, 
              400
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/a252e3f96dc54efc952eb9e433b6f924.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/a252e3f96dc54efc952eb9e433b6f924_thumb.png"
          }
        }, 
        "index": 24, 
        "published": 1414046272, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=84&sm=1&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9uZXdzLnlhaG9vLmNvbS91cy1sZWQtYWlyLXN0cmlrZXMtc3lyaWEta2lsbC01NTMtZmlyc3QtMTAyNDI4MDI0Lmh0bWwi.xiHRwR0joc3D8zjZXd1o7jN-ZFw&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=24", 
        "source": "http://news.yahoo.com/politics/", 
        "title": "US-led strikes kill more than 500 militants in Syria", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=84&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9uZXdzLnlhaG9vLmNvbS91cy1sZWQtYWlyLXN0cmlrZXMtc3lyaWEta2lsbC01NTMtZmlyc3QtMTAyNDI4MDI0Lmh0bWwi.xiHRwR0joc3D8zjZXd1o7jN-ZFw&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=24"
      }, 
      {
        "body": "MONROVIA, Liberia (AP) \u2014 Even as Liberians fall ill and die of Ebola, more than half the beds in treatment centers in the capital remain empty because of the government's order that the bodies of all suspected Ebola victims in Monrovia be cremated.\n\nCremation violates Liberians' values and cultural practices and the order has so disturbed people in the west African nation that the sick are often kept at home and, if they die, are secretly buried, increasing the risk of more infections\n\nPresident Ellen Johnson Sirleaf issued the cremation decree for Monrovia and the surrounding area in August, and the government has brought in a crematorium and hired experts. The order came after people in neighborhoods of the capital resisted burials of hundreds of Ebola victims near their homes.\n\nSince then, a recent analysis of space at Ebola treatment centers shows that of 742 beds available, more than half \u2014 391 \u2014 were vacant, said Assistant Health Minister Tolbert Nyenswah, who heads the government's Ebola response.\n\n\"For fear of cremation, do not stay home to die,\" Nyenswah admonished Liberians at a news conference last week.\n\nIn her statement declaring the state of emergency and the cremation order, Sirleaf acknowledged the edict runs contrary to national tradition. \"Ebola has attacked our way of life,\" she said.\n\nThat way of life includes honoring deceased ancestors.\n\nOn the second Wednesday of March each year, Liberians flock to cemeteries to honor their deceased loved ones on a public holiday known as National Decoration Day, scrubbing the headstones of relatives, clearing away brush from graves and decorating them with flowers and other mementoes.\n\nIn many parts of Liberia, tradition has also called for relatives to handle the bodies of loved ones before burial. Bodies are kept in the home for days or weeks, during which time people honor their loved ones by dancing around the corpse, washing it and cutting and braiding the hair. Before burial, church congregations also pray over the body.\n\nSince the latest outbreak of Ebola, these burial customs have been ordered halted when it comes to victims of the deadly virus because of the dangers they pose. The Ebola virus is spread through the body fluids of an infected person and can endure in corpses, posing a danger to those who handle them.\n\nGuidelines issued by the Centers for Disease Control and Prevention in the United States call for the bodies of Ebola victims to be handled only by those trained in handling infected human remains who are wearing the proper protective equipment. Bodies should be wrapped in plastic shrouds, then cremated or promptly buried in hermetically sealed caskets, the CDC says. The first person diagnosed with Ebola in the United States \u2014 a visitor from Liberia, Thomas Eric Duncan \u2014 died in Dallas this month, and his body was cremated.\n\nIn Liberia, the cremation edict in the capital and the order that Ebola victims elsewhere be buried in body bags in unmarked grave without relatives present has been met with resistance. Many find it hard to accept that they will never see the graves of those lost to the disease.\n\n\"We know cremation is not our culture in our country,\" Nyenswah said. \"But now we have disease, so we have to change the way we used to do business.\"\n\nAt least 4,665 people have been infected with Ebola in Liberia and 2,705 have died, according to the World Health Organization, which says there probably are more cases and deaths.\n\nNyenswah said many people are remaining home to die instead of reporting for treatment.\n\n\"We understand that there are secret burials taking place in the communities,\" he said. \"Let's stop that and report sick people and get them treated.\"\n\nAmid the new regulations, mortuaries and casket makers have lost business.\n\n\"For the last two months it has been difficult to sell even one casket a day,\" said Titus Mulbah, a proprietor at the Talented Brothers Casket Center in Monrovia. \"And this is all because all bodies now are considered Ebola bodies, as if other diseases are not killing people here.\"\n\nThere have been complaints that people who died of ailments other than Ebola have been cremated or buried anonymously. Television journalist Eddie Harmon said the body of his sister-in-law was hastily added to the bodies of Ebola victims and cremated, even though the family believes she died of hypertension.\n\n\"It is still paining us today because it was unjust and unfair,\" he said.\n\nIn neighboring Sierra Leone, families often picnic in cemeteries and clean graves on New Year's Day.\n\nSierra Leone has suffered 1,259 Ebola deaths by the latest WHO count. Unlike Liberia, the government has not ordered cremations, and Ebola treatment units in Sierra Leone have often been full.\n\nStill, there is the possibility that loved ones might be buried in unmarked graves and some families observe traditional practices in which mourners wash and lay hands on the body.\n\nAnthony Banbury, head of the U.N. Mission on Ebola Emergency Response, said people must change.\n\n\"The world has never seen a serious, grave and complex crisis of this nature where people are dying every day with unsafe burial practices,\" he said in Freetown, the Sierra Leone capital.\n\nA commentary on a website, Sierra Leone News Hunters, suggested that a memorial site be built to honor the dead who do not receive traditional burial rites, and to provide some comfort to their families.\n\n\"The erection of a monument bearing the names of all Ebola victims would not take away the sad memories but it would at least pacify the broken heart somewhat,\" it said.\n\nAssociated Press reporter Clarence Roy-Macaulay in Freetown, Sierra Leone, and AP medical writer Mike Stobbe in New York contributed to this report.", 
        "images": {
          "medium": {
            "size": [
              500, 
              332
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/1595d1b9e7d0489bb9c0ba71f3b47fb2_medium.png"
          }, 
          "original": {
            "size": [
              600, 
              399
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/1595d1b9e7d0489bb9c0ba71f3b47fb2.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/1595d1b9e7d0489bb9c0ba71f3b47fb2_thumb.png"
          }
        }, 
        "index": 25, 
        "published": 1414078765, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=85&sm=1&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9uZXdzLnlhaG9vLmNvbS9jcmVtYXRpb24tZmVhcnMtbGVhdmUtZW1wdHktZWJvbGEtYmVkcy1saWJlcmlhLTE5MzkyNTk5NC5odG1sIg.pDABO7x27gMdyLPteC3l7YgqJGs&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=25", 
        "source": "http://news.yahoo.com/health/", 
        "title": "Cremation fears leave empty Ebola beds in Liberia", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=85&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9uZXdzLnlhaG9vLmNvbS9jcmVtYXRpb24tZmVhcnMtbGVhdmUtZW1wdHktZWJvbGEtYmVkcy1saWJlcmlhLTE5MzkyNTk5NC5odG1sIg.pDABO7x27gMdyLPteC3l7YgqJGs&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=25"
      }, 
      {
        "body": "One afternoon during Labor Day weekend, a group of 15 or so Yale freshmen met in a classroom where history and French classes would soon be held. As they snacked on pretzels and Skittles, a few volunteered to act out a series of scenarios in which one student asks another out for frozen yogurt. In the first bit of role playing, one student was told to make it clear, in an easygoing way, that he or she wants to go out. The recipient of the invitation was told that he or she also wants to go but has a paper due. \u201cHow can you show enthusiasm while still turning down the invitation?\u201d a prompt on a card asked. The answer generally wasn\u2019t hard to convey or, for the freshmen watching, to interpret. Most students found that they knew how to demur while keeping the door open for next time.\n\nIn the second scenario, the stakes rose. Now the inviter must get the other person to the frozen-\u00adyogurt shop. And the invitee does not want to go, although \u2014 like most of us \u2014 he or she doesn\u2019t want to be rude. \u201cHow would your character handle this unwanted invitation?\u201d the second card read. The interaction made everyone in the room uncomfortable, as the inviter grew increasingly persistent and the invitee tried to fend the other off.\n\nThe intended lesson of this 90-minute workshop was that the line between a request and a demand, welcome interest and unwanted pressure, is usually fairly obvious. \u201cThis is the skill set people hammer out as little kids,\u201d says Melanie Boyd, an assistant dean of student affairs. She wants students to realize that they know how to recognize agreement, refusal and ambiguity.\n\nThe workshop reinforced policies, newly adopted by a growing number of universities, requiring students to make sure they have continuing affirmative consent for every phase of a sexual encounter. The policies, many of which have gone into effect in the last year, were created to help clarify internal university investigations of sexual-assault accusations. In the past, the main question was whether the person (usually a woman) who claimed that she was raped had made it clear that she said no (\u201cNo means no\u201d). The new rule shifts the inquiry to whether the student accused of assault got a signal of consent (\u201cYes means yes\u201d). In California, Gov. Jerry Brown recently signed an affirmative-consent bill, making \u201cyes means yes\u201d the standard at the state\u2019s colleges and universities. To continue to receive state funds for student financial aid, California institutions investigating allegations of sexual assault must determine whether both parties gave \u201caffirmative, conscious and voluntary agreement.\u201d Lack of resistance and silence no longer constitute proof of consent.\n\n\u201cYes means yes\u201d is part of a new conversation on campus. When I was a Yale student more than 20 years ago, I remember a few women setting up a microphone, after a Take Back the Night march, to tell stories of what we called date rape. But I don\u2019t remember anyone thinking the university would do anything about it. Ten years ago, I wrote about a handful of women who wanted better treatment from Yale, but their complaints seemed isolated and not much came of them. Then beginning around 2011, student activists from across the country started going public. They found one another online, called themselves survivors and demanded that their institutions change. And now everyone is talking about the problem, including President Obama.\n\nThe activism has forced not just administrators, faculty members and politicians to reckon with what goes on when students have sex, but also young men on campus. The White House wants them to sign on to a campaign called It\u2019s on Us. Fraternities are holding training sessions about preventing sexual assault (as many cope with related investigations and lawsuits). At Yale, students are required to participate in multiple workshops on sexual misconduct. \u201cYou can\u2019t go on Facebook or Twitter for 10 minutes without seeing a post about these issues,\u201d a 19-year-old English major told me.\n\nHe was confidently navigating the cultural shift. \u201cAsking, \u2018Are you O.K. with this?\u2019 doesn\u2019t have to be uncomfortable,\u201d he said. \u201cAnd in the aftermath, it\u2019s huge. You have a more positive memory of having sex with that person, because you don\u2019t feel worried.\u201d\n\nBut most male students expressed some nervousness about accidentally running afoul of consent rules, especially because drinking usually precedes a casual hookup. \u201cIt creates a crazy gray area that scares the hell out of everyone,\u201d one 21-year-old economics major told me. Some wondered whether training can really prepare you for what is often sex between relative strangers. One freshman woman explained the complicated dynamic by telling me about another freshman-orientation workshop, this one on intimacy. She was startled to hear several men say that they found holding hands more intimate than getting a hand job. The male students I talked with pointed out that holding hands, especially in public, is something you do when you are in a relationship, while a hand job could happen during a hookup. In theory, when it comes to sex, it might make sense to talk about what the other person wants as it\u2019s happening. But to do so, you might have to be a little bit tender, a little bit vulnerable. It\u2019s hard to have that sort of conversation if there\u2019s no intimacy.\n\n\u201cIt would be much more gratifying, and in both parties\u2019 best interest, for both the girl and guy to be straightforward \u2014 \u2018Hey, I\u2019m willing to do this,\u2019 \u201d a 19-year-old male water-polo player said. \u201cAnd yet the vocabulary for it is not really there.\u201d Affirmative-consent policies try to address this by recognizing body language as a form of consent. But to most of the men I talked to, this seemed like an invitation to more ambiguity, not less.\n\nOne area where the men were more at ease was \u201cbystander intervention.\u201d Universities know that probably the biggest threat to women on campus comes from a small group of serial predators who, research suggests, are responsible for most assaults. Some institutions, like Yale, are training students to watch for warnings signs that someone might be at risk. Sophomores take a workshop in which they watch an eight-minute video of a girl who goes out dancing, drinks to the point of bleary-eyed obliteration and lets a guy take her into a bedroom, where he forebodingly shuts the door. The second half of the video rewinds, noting the points at which a friend, a bartender, a stranger or a roommate could have stepped in to protect her. The interventions mostly aren\u2019t lengthy or heroic. They\u2019re small moments, and students are encouraged to be alert to indications that someone is exerting or feeling sexual pressure and to feel comfortable stepping in.\n\nAnd they do. Every male student I talked to had a story about intervening on the dance floor or at a party, mostly by just saying hello to someone who looked like a target of unwanted aggressive attention. The students said they looked out for their friends. They said they looked out for nonfriends who seemed headed for drunken trouble. As observers of a potentially fraught sexual encounter, if perhaps not as participants, they did know how to ask, \u201cAre you O.K. with this?\u201d \u201cDoing that yourself is way more awkward than doing it as a bystander,\u201d a 20-year-old rugby player said.\n\nIn the quest for a safer campus, it probably comes more naturally to institutions to help students learn prevention than to adjudicate disputes over consent after the fact. Education has always been the business of universities, and while federal law requires those that receive federal funds to make investigating and responding to sexual-assault complaints their business too, it\u2019s not easy. Even as survivors push for more protections for victims, other groups \u2014 including more than two dozen Harvard law professors, in a recent statement \u2014 are challenging new disciplinary procedures, saying they are unfairly stacked against those accused of sexual assault. This is difficult territory to get right. But for the first time, at some universities throughout the country, relative indifference has given way to dead seriousness.", 
        "images": {
          "medium": {
            "size": [
              500, 
              281
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/7870d1b56cde42cb88f7978551002172_medium.png"
          }, 
          "original": {
            "size": [
              600, 
              338
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/7870d1b56cde42cb88f7978551002172.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/7870d1b56cde42cb88f7978551002172_thumb.png"
          }
        }, 
        "index": 26, 
        "published": 1414001820, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=47&sm=1&a_id=tr1ca1ca1&url_id=.eJwNyEEOwjAMBMC_9O64rRAHfmMFt7GonYhsieD1ZY4zFaA9mMcYKb4w155ydV7n5cbLzOudXXb5WSiXWl8WO52NBCRBsm32doF9lHKNrgHK4u3sZOj_8nZYFugzFfgxXSA8JxY.vvSmvTG7jRhE9thGQdEl0F960zo&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=26", 
        "source": "http://digg.com/", 
        "title": "Hooking Up At An Affirmative Consent Campus", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=47&a_id=tr1ca1ca1&url_id=.eJwNyEEOwjAMBMC_9O64rRAHfmMFt7GonYhsieD1ZY4zFaA9mMcYKb4w155ydV7n5cbLzOudXXb5WSiXWl8WO52NBCRBsm32doF9lHKNrgHK4u3sZOj_8nZYFugzFfgxXSA8JxY.vvSmvTG7jRhE9thGQdEl0F960zo&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=26"
      }, 
      {
        "body": "Gathering your team in a soulless conference room staring at a white board is not where colorful ideas come from. Getting together with friends over a bottle of wine (or two) is equally inefficient. Creative name ideas don\u2019t materialize out of thin air. Nor do they come from games of Drunken Scrabble, Ouija boards and Magic 8 Balls.\nAs a brand name expert, with clients including Disney, Frito-Lay, Microsoft, and TaylorMade Golf, I\u2019ve had to come up with thousands of name ideas over the last 10 years. What I know for sure is that the single most powerful brainstorming resource is the Internet. And the ideal number of people is one: you. While brainstorming solo sounds counter-intuitive, my method is highly effective and you will be surprised and excited by how many good ideas you will generate and how quickly you will do it.\nHere are five of my most lucrative online brainstorming tools and techniques:\n1. Open the thesaurus treasure chest.\nBegin your online brainstorming on a thesaurus website, where you can find a jackpot of synonyms and related words. My go-to one is Thesaurus.com. When I had to come up with fresh name ideas for a hip frozen yogurt franchise in Utah that was targeted at teenagers, I hit the jackpot when I typed in the word \u201ccold\u201d and found these three fun names:\nBitter: With one of the two yogurt flavors being tart, it was self-deprecating and fun Goosebumps: Perfect for their target audience of hormonal teenagers Frigid: Playful and fun. We actually used this later as the name of an ice cream store\n2. Comb through glossaries of terms.\nEvery sport, hobby and industry has its own lingo of fun words and phrases. You can find pages and pages of them online by searching for \u201cglossaries,\u201d \u201clingo,\u201d \u201cvernacular,\u201d \u201cjargon,\u201d \u201cdictionaries,\u201d \u201cthesaurus,\u201d \u201cterms,\u201d \u201cwords\u201d or \u201cslang,\u201d which are essentially the same thing but will turn up different results in searches. While brainstorming frozen yogurt store names, I looked at snowboarder glossaries and stumbled upon the word \u201cChatter,\u201d which was perfect for this business, as it evokes teens socializing with each other.\n3. Go \"Googlestorming.\"\nThere are endless ways to utilize Google for brainstorming, or as I call it, \u201cGooglestorming.\u201d For the frozen yogurt store, I searched for \u201ccoldest places on earth.\u201d I found a small town \u201cdeep Siberian wilderness.\u201d The word Siberian jumped out at me. \u201cSiberia,\u201d is a funny word that would make a super name for the frozen yogurt store. It implies \u201ccold,\u201d and considering that Utah is a kind of Siberia (removed from the rest of the population), it\u2019s just the kind of hip name that teens would love. \u201cMom, I\u2019m going to Siberia with my friends.\u201d Cool.\n4. Tune into iTunes.\nSong titles make super sticky names, because just like the songs themselves, they get stuck in our head. While looking for frozen yogurt store names, I typed in the word \u201ccold,\u201d and discovered \u201cCold Hearted\u201d and \u201cCold Play,\u201d which could be fun. \u201cFunky Cold Medina,\u201d not so much. One of my favorite \u201ciTunes-inspired names,\u201d was for a hunky chili pepper-infused brownie. I did a song search for the word \u201cburn,\u201d and found the famous Elvis Presley song, \u201cBurning Love.\u201d The brownie flavor name became \u201cHunka Hunka Burning Love,\u201d and made everyone smile.\n5. Search stock photos and Google images.\nA picture says a thousand words. Photos can inspire awesome names, which is why I always do image searches to fuel my creativity. Stock photo websites such as Bigstock and Getty Images are fantastic places to get ideas and search for concepts related what you\u2019re naming. For the frozen yogurt store, I went to Google Images and searched for \u201ceat frozen yogurt,\u201d which led me to a lot of photos of colorful plastic spoons in yogurt, which immediately made me think of the phrase, \u201cSpoon Me,\" which ended up being the name the client chose.\nThere are many word and image resources online to help stimulate your creativity. Try the ones above and poke around to find others. You\u2019ll have the freedom to come up with ideas without anyone shooting them down. And you won\u2019t have to buy anyone dinner.", 
        "images": {
          "medium": {
            "size": [
              500, 
              319
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141216/5045d788b190445c9c3348f25b39120d_medium.png"
          }, 
          "original": {
            "size": [
              610, 
              390
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141216/5045d788b190445c9c3348f25b39120d.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141216/5045d788b190445c9c3348f25b39120d_thumb.png"
          }
        }, 
        "index": 27, 
        "published": 1413568800, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=on1ca1ca1&url_id=Imh0dHA6Ly93d3cuZW50cmVwcmVuZXVyLmNvbS9hcnRpY2xlLzIzODYwMSI.GuZ97-E-KKXkhMA2boQAdKF2Uvs&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=27", 
        "source": "http://www.entrepreneur.com/", 
        "title": "5 Must-Use Tools for Brainstorming Company Names", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=on1ca1ca1&url_id=Imh0dHA6Ly93d3cuZW50cmVwcmVuZXVyLmNvbS9hcnRpY2xlLzIzODYwMSI.GuZ97-E-KKXkhMA2boQAdKF2Uvs&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=27"
      }, 
      {
        "body": "Ottawa (AFP) - The shooter who rampaged through Canada's parliament was in Ottawa applying for a passport to travel to war-torn Syria and there was no connection to an attack earlier this week, the federal police commissioner said Thursday.\n\nThe man's killing of a soldier at a cenotaph in the city's downtown and storming of nearby parliament Wednesday were not linked to the deadly attack on a soldier in Quebec two days earlier, Royal Canadian Mounted Police Commissioner Bob Paulson told a news conference.\n\nInvestigators determined that the suspect in Wednesday's shooting, identified by Paulson as Michael Zehaf-Bibeau, had been in Ottawa since October 2 \"to deal with a passport issue.\"\n\n\"He was... hoping to leave for Syria,\" the nation's top cop said, adding that Zehaf-Bibeau's travel plans were gleaned from the man's estranged mother.\n\n\"There were concerns at the initial stage of the emergency response that there may have been more than one individual involved,\" Paulson said.\n\nBut both the RCMP and Ottawa police agreed \"that yesterday Zehaf-Bibeau acted alone,\" he said.\n\nIt remains unclear whether Zehaf-Bibeau \"received any support in the planning of his attack,\" he added.\n\nPolice are also trying to piece together how he got his hands on a Winchester lever action shot gun, since he was restricted from owning any firearms due to past criminal convictions for drug possession and uttering threats in a mugging.\n\nPaulson dismissed as a coincidence any link to the running over of two soldiers in a Quebec supermarket parking lot on Monday.\n\n\"We have no information linking the two attacks this week in Saint-Jean-sur-Richelieu and in Ottawa,\" Paulson said.\n\nFuthermore, \"our investigation has not revealed any link between Zehaf-Bibeau and Martin Couture Rouleau,\" he added.\n\nCouture-Rouleau, the driver in the parking lot attack, was shot dead by police after crashing his car and brandishing a knife.\n\nCouture-Rouleau had also sought to travel to Turkey to join the Islamic State group in neighboring Syria, but authorities seized his passport at the airport to prevent him from leaving.\n\nBoth the Monday and Wednesday attacks followed the deployment of Canadian fighter jets to join US-led airstrikes on the Islamic State in Iraq.", 
        "images": {
          "medium": {
            "size": [
              500, 
              305
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/0da259ffb08f49c4b8e5e482eb5b5d4e_medium.png"
          }, 
          "original": {
            "size": [
              600, 
              366
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/0da259ffb08f49c4b8e5e482eb5b5d4e.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/0da259ffb08f49c4b8e5e482eb5b5d4e_thumb.png"
          }
        }, 
        "index": 28, 
        "published": 1414084049, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=92&sm=1&a_id=tt1to1da1&url_id=Imh0dHA6Ly9uZXdzLnlhaG9vLmNvbS9jYW5hZGEtc2hvb3Rlci1wbGFubmVkLXN5cmlhLXBvbGljZS0yMTA1MzM5OTIuaHRtbCI.DQGkhBq5FKlppJcUNQFu2Ve0i-Q&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=28", 
        "source": "http://news.yahoo.com/politics/", 
        "title": "Canada shooter planned to go to Syria: police", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=92&a_id=tt1to1da1&url_id=Imh0dHA6Ly9uZXdzLnlhaG9vLmNvbS9jYW5hZGEtc2hvb3Rlci1wbGFubmVkLXN5cmlhLXBvbGljZS0yMTA1MzM5OTIuaHRtbCI.DQGkhBq5FKlppJcUNQFu2Ve0i-Q&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=28"
      }, 
      {
        "body": "But you don\u2019t need to be scared that the deadly disease carries an automatic death sentence \u2014 especially in the United States.\n\nAs I wrote earlier this week, the Ebola survival rate in the United States was 80% after the first five cases and bound to improve. And it did, after NBC News cameraman Ashoka Mukpo was discharged from Nebraska Medical Center. (Mukpo had contracted Ebola while working for NBC News in Liberia.)\n\nThat adds up to six U.S. Ebola patients with known clinical outcomes: Five survivors, one deceased. And that raises the Ebola survival rate in America to 83%.\n\nAlso See: The Ebola Number You Haven\u2019t Heard: More Than 80% Of U.S. Patients Have Survived\n\nTwo nurses who contracted Ebola in Dallas also are on the road to recovery.\n\nOn Tuesday, officials announced that nurse Nina Pham had been upgraded to \u201cgood condition\u201d at the National Institutes of Health, 10 days after her Ebola diagnosis. On Wednesday, nurse Amber Vinson was reported to be \u201cEbola-free\u201d by her caregivers at Emory University Hospital, according to Vinson\u2019s family. (As of press time, Emory hadn\u2019t confirmed the report.)\n\nTo put it another way: There may be only one U.S. patient left with Ebola \u2014 and she\u2019s getting better.\n\nIt\u2019s an impressive run of good health and, perhaps, good fortune. And a high U.S. survival rate is notable for two reasons.\n\n1. The current Ebola survival rate in Africa is just 30% to 40%. 2. Only a week ago, some pundits were predicting a mass outbreak of Ebola in the United States. As the days pass, with no more U.S. Ebola patients and no more deaths, that worst-case scenario begins to look more and more unlikely. And the best-case scenario \u2014 that the United States has weathered a public health crisis and will be stronger for it \u2014 is starting to become more realistic, too.\n\nThere are caveats upon caveats here. Six Ebola patients, or even eight if you count the two nurses, is a small sample size. Not every American is out of quarantine yet (here\u2019s a map of who\u2019s been exposed to Ebola), and Pham and Vinson aren\u2019t even out of the hospital.\n\nAnd Ebola remains quite terrifying. The deadly disease is highly infectious and can leave survivors weak for months to come.\n\nYet facts are facts, too. At least three Ebola patients \u2014 Kent Brantly, Nancy Writebol, and a World Health Organization doctor who\u2019s asked to be kept anonymous \u2014 were critically ill after getting sick in Africa. They\u2019ve since pulled through after receiving care at Emory.\n\nAs Emory\u2019s infectious disease chief pointed out, most patients might even be able to survive Ebola, based on what public health officials are starting to discover from treating the disease in the United States.\n\nYes, Ebola Is Scary. But It\u2019s Also Beatable. Here\u2019s Why.\n\nIt\u2019s tempting to suggest that U.S. hospitals have some sort of blueprint to treat Ebola, but that\u2019s not quite right. Rather, the U.S. Ebola patients experienced somewhat different courses of care. They had different speed to diagnosis, took different experimental drugs. Some, like Nancy Writebol and Rick Sacra, were in their 50s. Others, like Ashoka Mukpo, were relatively young and healthy.\n\nBut one commonality stands out. The five U.S. Ebola patients who recovered were taken to the nation\u2019s top biocontainment facilities. Hospitals that had expertise, training, and the ability to devote many staff to round-the-clock Ebola patient care.\n\nThe U.S. Ebola patient who didn\u2019t make it \u2014 Thomas Duncan, the first person every diagnosed with Ebola in America \u2014 never left his local Texas hospital. Duncan\u2019s sad death, and his infection of two nurses, may end up as a signal moment in American public health and emergency response. It catalyzed new, stricter CDC protocols. It changed the thinking on whether all hospitals were really equipped to handle a dangerous outbreak. It led to the creation of a full-time national team of rapid responders.\n\nWhen the United States has to deal with its next public health crisis, expect to see this more coordinated response kick into gear.\n\nAnd that might be needed sooner than later, because Ebola isn\u2019t going away. Tens of thousands remain sick or at risk in West Africa, and the longer there\u2019s an Ebola hotspot on any part of the globe, the worse it will be for the rest of the world.\n\nBut for now, U.S. residents can take some comfort.\n\nEbola came to America. And America is beating Ebola back.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/4b9e85fd31744d7f9354ec105061efab_medium.png"
          }, 
          "original": {
            "size": [
              1024, 
              828
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/4b9e85fd31744d7f9354ec105061efab.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/4b9e85fd31744d7f9354ec105061efab_thumb.png"
          }
        }, 
        "index": 29, 
        "published": 1414046700, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=92&sm=1&a_id=tt1to1da1&url_id=.eJwNzDsSgzAMBcC70D8EJFVuI2Ml1sS_sQRMbh_aLXZK7v1FdF3X_G4jiM17K2TqYhS5RuXSaqRtWZ-0LrQ9iIsM3RlqCMKu9QMJLTPklPFDv0mqw_krFd7AFZLvDwcMqVlX54zEBjvGqadEmv6cBjAk.RrHFqMrRxYzEohnqmWfQAsYtKOY&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=29", 
        "source": "http://forbes.com/", 
        "title": "America Is Beating Ebola: Every Patient Taken To An Elite U.S. Hospital Has Survived.", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=92&a_id=tt1to1da1&url_id=.eJwNzDsSgzAMBcC70D8EJFVuI2Ml1sS_sQRMbh_aLXZK7v1FdF3X_G4jiM17K2TqYhS5RuXSaqRtWZ-0LrQ9iIsM3RlqCMKu9QMJLTPklPFDv0mqw_krFd7AFZLvDwcMqVlX54zEBjvGqadEmv6cBjAk.RrHFqMrRxYzEohnqmWfQAsYtKOY&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=29"
      }, 
      {
        "body": "A majority of the public supports British warplanes, armed drones and special forces being used to fight Islamic State (Isis) in Syria as well as Iraq, a survey reveals today.\n\nThere is also strong backing for deploying small numbers of ground troops in an advisory and training role in Iraq, according to the YouGov data. The support for such training missions inside Syria was also relatively high at 49 per cent of those polled.\n\nThe renewed public appetite for intervention was in stark contrast to August 2013 when parliament rejected military action against the Assad regime in Syria, said Joel", 
        "images": {
          "medium": {
            "size": [
              140, 
              93
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/444da033d60a4ec5a8728df93c6b37b8.png"
          }, 
          "original": {
            "size": [
              140, 
              93
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/444da033d60a4ec5a8728df93c6b37b8.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/444da033d60a4ec5a8728df93c6b37b8_thumb.png"
          }
        }, 
        "index": 30, 
        "published": 1414022460, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=84&sm=1&a_id=ve1ve1de1&url_id=Imh0dHA6Ly93d3cudGhldGltZXMuY28udWsvdHRvL25ld3MvdWsvZGVmZW5jZS9hcnRpY2xlNDI0NDg1Ny5lY2Ui.FEXg9GX1W6fpbI3jjW9gIx5r14Q&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=30", 
        "source": "http://thetimes.co.uk/", 
        "title": "Support for airstrikes on Isis in Syria is growing", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=84&a_id=ve1ve1de1&url_id=Imh0dHA6Ly93d3cudGhldGltZXMuY28udWsvdHRvL25ld3MvdWsvZGVmZW5jZS9hcnRpY2xlNDI0NDg1Ny5lY2Ui.FEXg9GX1W6fpbI3jjW9gIx5r14Q&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=30"
      }, 
      {
        "body": "His doctor drove him over the border. It was quicker that way: if the man donated in Switzerland, his blood would be delayed while paperwork was filled out and authorisations sought.\n\nThe nurse in Annemasse, France, could tell from the label on the blood bag destined for Paris that this blood was pretty unusual. But when she read the details closely, her eyes widened. Surely it was impossible for this man seated beside her to be alive, let alone apparently healthy?\n\nThomas smiled to himself. Very few people in the world knew his blood type did \u2013 could \u2013 exist. And even fewer shared it. In 50 years, researchers have turned up only 40 or so other people on the planet with the same precious, life-saving blood in their veins.\n\nRed blood cells carry oxygen to all the cells and tissues in our body. If we lose a lot of blood in surgery or an accident, we need more of it \u2013 fast. Hence the hundreds of millions of people flowing through blood donation centres across the world, and the thousands of vehicles transporting bags of blood to processing centres and hospitals.\n\nIt would be straightforward if we all had the same blood. But we don\u2019t. On the surface of every one of our red blood cells, we have up to 342 antigens \u2013 molecules capable of triggering the production of specialised proteins called antibodies. It is the presence or absence of particular antigens that determines someone\u2019s blood type.Discovering new blood groups\n\nSome 160 of the 342 blood group antigens are \u2018high-prevalence\u2019, which means that they are found on the red blood cells of most people. If you lack an antigen that 99 per cent of people in the world are positive for, then your blood is considered rare. If you lack one that 99.99 per cent of people are positive for, then you have very rare blood.\n\nIf a particular high-prevalence antigen is missing from your red blood cells, then you are \u2018negative\u2019 for that blood group. If you receive blood from a \u2018positive\u2019 donor, then your own antibodies may react with the incompatible donor blood cells, triggering a further response from the immune system. These transfusion reactions can be lethal.\n\nBecause so few people have it, by definition, rare blood is hardly ever needed. But when it is, finding a donor and getting the blood to a patient in crisis can become a desperate race against the clock. It will almost certainly involve a convoluted international network of people working invisibly behind the bustle of \u2018ordinary\u2019 blood donation to track down a donor in one country and fly a bag of their blood to another.\n\nForty years ago, when ten-year-old Thomas went into the University Hospital of Geneva with a routine childhood infection, his blood test revealed something very curious: he appeared to be missing an entire blood group system.\n\nThere are 35 blood group systems, organised according to the genes that carry the information to produce the antigens within each system. The majority of the 342 blood group antigens belong to one of these systems. The Rh system (formerly known as \u2018Rhesus\u2019) is the largest, containing 61 antigens.\n\nThe most important of these Rh antigens, the D antigen, is quite often missing in Caucasians, of whom around 15 per cent are Rh D negative (more commonly, though inaccurately, known as Rh-negative blood). But Thomas seemed to be lacking all the Rh antigens. If this suspicion proved correct, it would make his blood type Rh \u2013 one of the rarest in the world, and a phenomenal discovery for the hospital haematologists.\n\nRh blood was first described in 1961, in an Aboriginal Australian woman. Until then, doctors had assumed that an embryo missing all Rh blood cell antigens would not survive, let alone grow into a normal, thriving adult. By 2010, nearly five decades later, some 43 people with Rh blood had been reported worldwide.\n\nHardly able to believe what she was seeing, Dr Marie-Jos\u00e9 Stelling, then head of the haematology and immunohaematology laboratory at the University Hospital of Geneva, sent Thomas\u2019 blood for analysis in Amsterdam and then in Paris. The results confirmed her findings: Thomas had Rh blood. And with that, he had instantly become infinitely precious to medicine and science.\n\nResearchers seeking to unravel the mysteries of the physiological role of the intriguingly complex Rh system are keen to get hold of Rh blood, as it offers the perfect \u2018knockout\u2019 system. Rare negative blood is so sought after for research that even though all samples stored in blood banks are anonymised, there have been cases where scientists have tried to track down and approach individual donors directly to ask for blood.Inside the blood factory\n\nAnd because Rh blood can be considered \u2018universal\u2019 blood for anyone with rare blood types within the Rh system, its life-saving capability is enormous. As such, it\u2019s also highly prized by doctors \u2013 although it will be given to patients only in extreme circumstances, and after very careful consideration, because it may be nigh on impossible to replace. \u201cIt\u2019s the golden blood,\u201d says Dr Thierry Peyrard, the current Director of the National Immunohematology Reference Laboratory in Paris.\n\nBlood groups are inherited, and Rh is known to run in families. So the next step for the haematologists in Geneva was to test Thomas\u2019 family in the hope of finding another source, particularly as Thomas wouldn\u2019t be able to donate until he turned 18. Things looked even more hopeful when it turned out Thomas\u2019 grandfathers were third-degree cousins. But the tests showed Thomas\u2019 Rh blood was due to two completely different random mutations on both sides. Pure chance, twice over, in the face of vanishingly small odds.\n\nIn 2013, Walter Udoeyop received a letter from an old friend back in Nigeria. Father Gerald Anietie Akata\u2019s 70-year-old mother had a tumour in her heart, but no hospital in Nigeria could perform the surgery she needed. Akata enclosed his mother\u2019s medical records, asking for Walter\u2019s help.\n\nWalter, a consultant at Johnson City Medical Center, Tennessee, knew from the start this wasn\u2019t going to be easy. Francisca Akata\u2019s operation would cost a daunting $150,000 minimum if she had it in the USA. Father Akata had been a pastor in Johnson City for several years, and Walter initially hoped to enlist the help of the church and hospitals his friend had served in. But neither could raise such a large amount of money.\n\nHe recalled that another friend had recently had open-heart surgery in the United Arab Emirates (UAE) for only $20,000. He phoned the hospital there, and the staff agreed to operate on Francisca. Father Akata\u2019s parishioners in the USA and Nigeria raised the money, and three months later, Francisca Akata was flying eastwards towards the UAE.\n\nBut a few days after her admission, the doctors told Francisca that blood tests had revealed that she had a rare blood type, shared by 0.2 per cent of the white population: Lutheran b negative. To complicate the matter, she was also O negative \u2013 the uncommon, but not officially rare blood type that many of us have heard of, shared by around 5 per cent of people. The combination made Francisca\u2019s blood so rare it would be difficult, if not impossible, to find a match for her.\n\nSince there was no compatible blood in the UAE or any of the other Gulf States, Mrs Akata had to fly back home and wait until matching blood was found. The hospital searched for blood but couldn\u2019t find any in the two weeks that followed.\n\nWalter requested Francisca\u2019s blood tests from the hospital and then began the search for compatible blood in the USA. He tried blood centre after blood centre across the country before he was referred to the American Rare Donor Program in Philadelphia, a database of all rare blood donors in America. Finally, he had located some suitable donors.\n\nHis relief was short lived because, as Thomas or Peyrard could have told him, it\u2019s a lot harder for blood to cross borders than it is for people. \u201cYou would not imagine how difficult it is when you have to import or export rare blood,\u201d Peyrard says. \u201cYour patient is dying, and you have people in an office asking for this paper and that form. It\u2019s just crazy. It\u2019s not a TV set, it\u2019s not a car. It\u2019s blood.\u201d\n\nSometimes sending blood from one country to another is more than a bureaucratic nightmare. As Walter now discovered, the hospital in the UAE had a policy not to accept blood donations from outside the Gulf States, which meant that Francisca wouldn\u2019t be able to use the blood he had found in America.\n\nThe situation looked bleak. But then, after a chance meeting with a colleague, Father Akata found out about a small general hospital in Cameroon, Nigeria\u2019s neighbour to the east, that had set up a heart surgery programme with funding from the Catholic Church. Walter got in touch with the surgeons there, who confirmed that they could do the surgery if he could supply compatible blood.\n\nThe American Rare Donor Program contacted the South African National Blood Service, which had four suitable donors listed; however, one of these was unreachable, one wasn\u2019t able to donate until later in the year, and two had been medically retired from donating. These are all common problems with rare donors. There are limits placed on how often people can donate. What\u2019s more, keeping track of donors can also be a challenge \u2013 some get ill or die, and others move home without updating the blood services.\n\nThere were two units of compatible blood in South Africa\u2019s frozen rare blood bank, but frozen blood has a 48-hour lifespan, compared to four weeks for fresh blood. If it got held up at customs, or delayed for any other reason, it would be unusable by the time it reached the hospital in Cameroon. To use the frozen South African blood, Francisca would have to have her operation in South Africa. Walter was running out of options.\n\nWhen he turned 18, Thomas was encouraged to donate blood for himself. There is now no frozen blood bank in Switzerland, so his blood is stored in the rare blood banks in Pari", 
        "images": {
          "medium": {
            "size": [
              500, 
              281
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/084bc3bc505b493b8149b95c05e00d11_medium.png"
          }, 
          "original": {
            "size": [
              800, 
              450
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/084bc3bc505b493b8149b95c05e00d11.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/084bc3bc505b493b8149b95c05e00d11_thumb.png"
          }
        }, 
        "index": 31, 
        "published": 1414002623, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=41&sm=1&a_id=tr1ca1ca1&url_id=Imh0dHA6Ly9tb3NhaWNzY2llbmNlLmNvbS9zdG9yeS9tYW4tZ29sZGVuLWJsb29kIg.39EsCihzlNI4XiT7kntVmF3VJFY&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=31", 
        "source": "http://digg.com/", 
        "title": "The Man With The Golden Blood", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=41&a_id=tr1ca1ca1&url_id=Imh0dHA6Ly9tb3NhaWNzY2llbmNlLmNvbS9zdG9yeS9tYW4tZ29sZGVuLWJsb29kIg.39EsCihzlNI4XiT7kntVmF3VJFY&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=31"
      }, 
      {
        "body": "Many of us entrepreneurs came up learning to focus our time on the traditional sales funnel. It was \u201cbuy or goodbye\u201d as we converted hot leads and prospects into customers.\nWe ignored past customers and took current customers for granted -- like partners we\u2019d been married to for 30 years and the last 29 hadn\u2019t been too great -- offering bright and shiny promotions to new buyers only.\nIf we only focus on those prospects ready to buy, we miss out on most of the opportunities to affect purchase decisions. We have so much information at our fingertips -- our path to purchase can be long and winding. Today we are ready to buy when, and only when, we hear about and find the right product.\nWhen endless information is at our fingertips, there is no standard time frame for purchase. Building relationships takes time and the kind of loyal customers that share brand stories cannot always be built overnight. We do business with people we know, like and trust. The best way to earn that position is by getting to know other people.\nToday, 60 percent of all purchase decisions are made before customers enter your funnel. Consumers come to you prepared and educated, with trusted referrals in hand before they ever hear your pitch. We can\u2019t have funnel vision. Instead, we need to focus on the sales cloud.\nThe sales cloud is made up of all the ways customers hear about your brand: blogs, reviews, trusted referrals, social media, your website. Your competitors are here too, with all of you vying for the attention of your market, trying to survive the sales cloud sieve. Here your market may or may not be hearing about you -- for better or for worse.\nThose sharing your brand story are past customers and anyone on whom your business has made an impression. As entrepreneurs we can\u2019t afford to miss out on sales-cloud impressions and we certainly can\u2019t go the way of treating this space as a waste of time.\nTrusted referrals are the best marketing. When customers pass through your company funnel, they don\u2019t go live on some deserted island somewhere (unless you sell deserted islands, of course) -- they go back into the mix. They share their experiences, good and bad.\nOnce we\u2019re ready to focus outside the funnel, we\u2019re ready for a whole new way of look at sales we call UnSelling. This is what happens when you understand the humanity of your market, produce a quality product, and create experiences that lead to trusted referrals in the sales cloud.\nIn the old funnel, prospects moved to customers, but now in the sales cloud prospects can be current customers, past customers and people having conversations that wouldn\u2019t be ready to buy in the next six weeks. Where do you have funnel vision?", 
        "images": {
          "medium": {
            "size": [
              500, 
              319
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141216/5a43355981f74d6ebcde2f0131d4bdaf_medium.png"
          }, 
          "original": {
            "size": [
              610, 
              390
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141216/5a43355981f74d6ebcde2f0131d4bdaf.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141216/5a43355981f74d6ebcde2f0131d4bdaf_thumb.png"
          }
        }, 
        "index": 32, 
        "published": 1413498600, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=on1ca1ca1&url_id=Imh0dHA6Ly93d3cuZW50cmVwcmVuZXVyLmNvbS9hcnRpY2xlLzIzODU4NiI.0yGN5YD7Ys60CoPwrc4VyHLVWsg&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=32", 
        "source": "http://www.entrepreneur.com/", 
        "title": "Entrepreneurs Can\u2019t Afford to Have Funnel Vision", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=on1ca1ca1&url_id=Imh0dHA6Ly93d3cuZW50cmVwcmVuZXVyLmNvbS9hcnRpY2xlLzIzODU4NiI.0yGN5YD7Ys60CoPwrc4VyHLVWsg&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=32"
      }, 
      {
        "body": "NEW YORK (Reuters) - The patient being tested for Ebola at a New York City hospital was identified as a doctor named Craig Spencer from Harlem, New York City Councilman Mark Levine said on Thursday.\n\nHours after Spencer was taken to Bellevue Hospital to undergo tests after complaining of fever and gastrointestinal discomfort, authorities were discussing possible evacuation of the Harlem apartment building where he lived, Levine said.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/788b7088ae344b1badb68e539f6235dd.png"
          }, 
          "original": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/788b7088ae344b1badb68e539f6235dd.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/788b7088ae344b1badb68e539f6235dd_thumb.png"
          }
        }, 
        "index": 33, 
        "published": 1414086365, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=85&sm=1&a_id=ve1ve1de1&url_id=.eJwFwUkKwCAMAMC_eI-ieGj7G5egUjUSA8Xfd0ZVkfUYM_Hb-oRKpBMNc4hfWEEaToGIbRYQ3IIZMFIPkBkSh1ZgL5wJGZx13lt33brK6OoHb_cedw.DHLpWwqcnnnBIw1ZCtzxVaxwfLY&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=33", 
        "source": "http://news.yahoo.com/health/", 
        "title": "New York patient being tested for Ebola is Dr. Craig Spencer", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=85&a_id=ve1ve1de1&url_id=.eJwFwUkKwCAMAMC_eI-ieGj7G5egUjUSA8Xfd0ZVkfUYM_Hb-oRKpBMNc4hfWEEaToGIbRYQ3IIZMFIPkBkSh1ZgL5wJGZx13lt33brK6OoHb_cedw.DHLpWwqcnnnBIw1ZCtzxVaxwfLY&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=33"
      }, 
      {
        "body": "Joni Ernst, career crackpot, veteran juggler of pig testicles, and determined foe of Agenda 21, the secret UN plot to steal all our golfs, seems to have gone into a kind of delay game as she edges toward the Senate election in Iowa. First, she's stopped doing almost any interviews with the editorial boards of Iowa's newspapers. Or even local TV. Perhaps she's down in the root cellar, stocking up the canned goods and keeping the crystal set in trim.\n\nI do so dig that last part -- \"...or whether it's from the government, should they decide that my rights are no longer important.\"\n\nShe's going to bring down an F-16 with her 9-mil, but she doesn't have the fortitude to stand up to the editorial board of the Cedar Falls Gazette.\n\nShe's leading in the polls, by the way.", 
        "images": {
          "medium": {
            "size": [
              362, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141222/f4e39aa410d6447793ab7eecd17bc0ac.png"
          }, 
          "original": {
            "size": [
              362, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141222/f4e39aa410d6447793ab7eecd17bc0ac.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141222/f4e39aa410d6447793ab7eecd17bc0ac_thumb.png"
          }
        }, 
        "index": 34, 
        "published": 1414059300, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=92&sm=1&a_id=tt1to1da1&url_id=Imh0dHA6Ly93d3cuZXNxdWlyZS5jb20vYmxvZ3MvcG9saXRpY3MvSm9uaV9UYWtlc19BX0RpdmUi.E1mPooRr7d5zIYkpwwBPg9d5Nrk&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=34", 
        "source": "http://esquire.com/", 
        "title": "Running Out The Clock", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=92&a_id=tt1to1da1&url_id=Imh0dHA6Ly93d3cuZXNxdWlyZS5jb20vYmxvZ3MvcG9saXRpY3MvSm9uaV9UYWtlc19BX0RpdmUi.E1mPooRr7d5zIYkpwwBPg9d5Nrk&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=34"
      }, 
      {
        "body": "About\nJoin Us\nLegalese", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/93cb657294724d63a96bfdaa253b747f_medium.png"
          }, 
          "original": {
            "size": [
              1200, 
              627
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/93cb657294724d63a96bfdaa253b747f.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/93cb657294724d63a96bfdaa253b747f_thumb.png"
          }
        }, 
        "index": 35, 
        "published": 1413991699, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=40&sm=1&a_id=tr1ca1ca1&url_id=.eJwVykEOwyAMBdG7ZP_DvrdxiFVbBYyCicXtk65GeppN3PsnpYjYZw-7XNaerSYXxklaFoZYoNKPBwjdtDnosOn4L3xYIXDXk6vml8hLgdDNaLQGLb4G3mj7wm1m2R6Nnire.j8FlVrOWMbsbQzy5L6BfhR41keY&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=35", 
        "source": "http://www.upworthy.com", 
        "title": "'The Daily Show' Makes A Point About The Ebola Epidemic That'll Have Naysayers Saying 'Touch\u00e9'", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=40&a_id=tr1ca1ca1&url_id=.eJwVykEOwyAMBdG7ZP_DvrdxiFVbBYyCicXtk65GeppN3PsnpYjYZw-7XNaerSYXxklaFoZYoNKPBwjdtDnosOn4L3xYIXDXk6vml8hLgdDNaLQGLb4G3mj7wm1m2R6Nnire.j8FlVrOWMbsbQzy5L6BfhR41keY&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=35"
      }, 
      {
        "body": "Sporting News has selected a Rookie of the Year since 1946, a year before MLB began its official award. This year's winners, as voted on by fellow players in their leagues, are Jacob deGrom of the Mets (National League) and Jose Abreu of the White Sox (American League).\n\nJacob deGrom, a ninth-round draft pick in 2010 and No. 10 prospect in the Mets\u2019 organization heading into 2014 according to Baseball America, is Sporting News' National League Rookie of the Year after a season that was as dominating as it was surprising.\n\nAnd that\u2019s saying something, because deGrom\u2019s season was really, really surprising.\n\nQuickly, the backdrop: The 6-4 right-hander was a shortstop for Stetson University before his coach switched him to the mound as a junior, and then he only made six starts in his first year with the Mets before missing a year with Tommy John surgery. After a good return split between low-A and high-A (2.43 ERA in 19 starts), deGrom had a rough 2013: he posted a 4.80 ERA in 10 starts at Double-A and a 4.52 ERA in 14 starts at Triple-A.\n\nThose aren\u2019t the types of numbers that scream \u201cRookie of the Year lock\u201d heading into spring training. But deGrom was solid in his first seven starts at Triple-A, and when the Mets needed someone to start against the Yankees on May 15, they gave him a shot.\n\nIn that start, deGrom went seven innings, struck out six, allowed just four hits, two walks and one run. He remained in the big-league rotation the rest of the season.\n\nGoing forward, deGrom really only had one short stretch of poor starts, four games where his ERA climbed from 1.83 to 4.39, but he spent pretty much the rest of the season chipping away at that number.\n\nBy the time his season ended, deGrom had a 2.69 ERA in 22 starts covering 140 1/3 innings. Among pitchers with at least 140 innings, deGrom\u2019s 2.67 FIP ranked ninth in all of baseball. Clearly, the players who voted for the SN award were impressed.\n\nFor most of the summer, it seemed Cincinnati speedster Billy Hamilton would run away with (pardon the pun) the NL award. Playing good defense and batting leadoff for the Reds, Hamilton stole 56 bases while batting .250. He was caught stealing 23 times, though, and his .292 on-base percentage shows he still has a ways to go.\n\n\"What (deGrom's) done, it is truly remarkable,\" Mets manager Terry Collins told The Wall Street Journal last month. \"I understand what a year Billy's had and what a year Kolten Wong has had. But I don't know if they're as good as my guy's been this year.\"\n\nPretty much everything about deGrom said he\u2019s ready to be a star, right now. Despite throwing a career-high innings (178 2/3 counting Triple-A) this year, deGrom was playing his best baseball at the end of the season.\n\nOn September 9, he threw eight shutout innings against the Rockies, allowing just three hits while striking out nine. In his next outing, deGrom struck out the first eight Marlins he faced, and he ended the game with 13 strikeouts in seven innings.\n\nThen, in his final start of the season, deGrom carried a perfect game into the fifth innings, striking out eight of Atlanta\u2019s first 12 batters.\n\nSo, yes, it\u2019s fair to say the way deGrom finished the season has the Mets excited about what\u2019s in store for the former shortstop next season.\n\nOther Mets to be honored as Sporting News Rookie of the Year include Jerry Koosman (1968), Jon Matlack (1972), Daryl Strawberry (1983) and Dwight Gooden (1984).\n\nMonday: AL and NL Rookies of the Year and AL and NL Comeback Players of the Year\n\nTuesday: AL and NL Managers of the Year", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141219/e5a16149e50d42eb90b85419b3ebe6c6_medium.png"
          }, 
          "original": {
            "size": [
              1280, 
              720
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141219/e5a16149e50d42eb90b85419b3ebe6c6.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141219/e5a16149e50d42eb90b85419b3ebe6c6_thumb.png"
          }
        }, 
        "index": 36, 
        "published": 1413801683, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=on1ca1ca1&url_id=.eJwdyEEOwyAMBMC_5L6BRD31Nya4hBZwZFwhfh-1c5zlNLuezo0x1n6JWm6p8ejrIdXVElw30el2vz2weez-l6BBGjv-28iyNCooTOnLUJFPZsgLdjImk-JNhwRETioVla0j5FImTqq5mDQox77cScgxWw.J-Z5w9a3OMWaLlOf2GqbaacHqyE&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=36", 
        "source": "http://sports.aol.com/fanhouse/", 
        "title": "Sporting News MLB awards 2014: Mets' Jacob deGrom voted top NL rookie", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=on1ca1ca1&url_id=.eJwdyEEOwyAMBMC_5L6BRD31Nya4hBZwZFwhfh-1c5zlNLuezo0x1n6JWm6p8ejrIdXVElw30el2vz2weez-l6BBGjv-28iyNCooTOnLUJFPZsgLdjImk-JNhwRETioVla0j5FImTqq5mDQox77cScgxWw.J-Z5w9a3OMWaLlOf2GqbaacHqyE&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=36"
      }, 
      {
        "body": "Our favorite resources for teaching digital citizenship\nIt's Digital Citizenship Week and Connected Educators Month, so in today's post we're focusing on how connected educators can teach digital citizenship. (Phew, is that enough buzzwords for you?) One of the best resources for teachers is the internet. And with the increased prevalence of mobile devices in education, internet access is expanding. We know that \"too many resources\" can also be a problem, and there are more than enough helpful sites to guide Digital Citizenship lessons. Here are some of our (FREE) favorites:\nYouTube: To say that YouTube offers a plethora of video resources is a severe understatement, as it currently facilitates the viewing of 6 billion hours of video every month (\"an hour for every person on Earth\", their site notes). They also have YouTubeCurriculum, a channel that offers videos on staying safe on YouTube, guarding your reputation and staying legal on copyright issues, to name a few. YouTube is often victim to blanket bans in schools, as there are many not-safe-for-school videos on the site, so this digital citizenship lesson is definitely useful.\nPinterest: Curating your own board of resources is nothing new to teachers. Pinterest's social nature enables easier discovery of tried and true educational resources, and teachers can easily see pins of many thought leaders in the digital citizenship space. Searching Pinterest can lead to new lesson plans, websites, and ways to reach students. We've started a digital citizenship board. Do you have one? Let us know, and we'll follow you!\nEdudemic: You'll find resources for teachers and students, almost all of them with a focus on keeping everyone legal, safe, and informed. There are many useful guides and blog posts we've found, and almost all of them highlight an aspect of digital citizenship.\nTeachinctrl: Provided by Cable in the Classroom, this site offers lesson-oriented information under several digital citizenship sub-topics (such as privacy and media literacy), each with a video and supporting lesson materials.\nAlso, for extra credit (to talk like a teacher!), taking part in Twitter Chats is an exciting and different way to explore the digital citizenship space. We invite you to join us in tomorrow night's #digcit Twitter Chat (to be moderated by @EdTechSandyK) at 7:00pm EST Wednesday. Join in and answer questions; you might even pick up some wisdom from other connected educators.", 
        "images": {
          "medium": {
            "size": [
              150, 
              150
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141219/ee524b6312584949ae16f1b741e0ffc3.png"
          }, 
          "original": {
            "size": [
              150, 
              150
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141219/ee524b6312584949ae16f1b741e0ffc3.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141219/ee524b6312584949ae16f1b741e0ffc3_thumb.png"
          }
        }, 
        "index": 37, 
        "published": 1413817527, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=70&sm=1&a_id=tt1to1da1&url_id=.eJwNxzEOgCAMAMC_sNeKcfI3WCs0UUpodfD1Ml0uFPe2Ie6XZpss2UR6I2l1ro7j1HCZ44pxHqI-Hc70ahdn6GzjxAandnBOVKRmOCSLpwtIXD6uVqRh-AFziyUv.e_SWILOnvTfKXeTCncxoo68mmu8&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=37", 
        "source": "http://blogs.sas.com/content/", 
        "title": "Our favorite resources for teaching digital citizenship", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=70&a_id=tt1to1da1&url_id=.eJwNxzEOgCAMAMC_sNeKcfI3WCs0UUpodfD1Ml0uFPe2Ie6XZpss2UR6I2l1ro7j1HCZ44pxHqI-Hc70ahdn6GzjxAandnBOVKRmOCSLpwtIXD6uVqRh-AFziyUv.e_SWILOnvTfKXeTCncxoo68mmu8&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=37"
      }, 
      {
        "body": "OTTAWA \u2014 At least two gunmen traumatized the heart of the Canadian government on Wednesday, with one shooting a military guard at the National War Memorial and then entering the adjacent Parliament building, where multiple rounds were fired. Shooting also was reported at a nearby shopping mall.\n\nPolice officers rushed to secure the Parliament building and move occupants to safety as they hunted for what Canadian news reports said were possibly two or three assailants, in what had the appearance of a coordinated attack.\n\nThe Canadian Broadcasting Corporation reported that one assailant was killed. The condition of the soldier who was shot was not immediately clear, with conflicting accounts. Witnesses reported earlier that they believed the soldier had been killed.\n\nMarc Coucy, a representative of the Ottawa Police Service, told the Canadian Broadcasting Corporation that officers were looking for \u201cmultiple suspects\u201d in shootings at three locations.\n\nThe United States Embassy in Ottawa also reported it was in lockdown mode, in an advisory to American citizens posted on its website.\n\nThe shootings came amid heightened concern about terrorist attacks in Canada, two days after a Muslim convert, a radical jihadist, ran over two soldiers at a suburban Montreal strip mall, killing one of them. Prime Minister Stephen Harper, an outspoken critic of the Islamic State movement and other militant groups, has been considering the introduction of new antiterrorism legislation.\n\nThe shootings in Ottawa began about 10 a.m., just as the leaders of Parliament were holding their weekly meetings, suggesting the possibility of the attack being deliberate timed. Many of the lawmakers were rushed into secure rooms in the basement by guards.\n\n\u201cI heard the shots as I was walking into a conference meeting,\u201d said Chrystia Freeland, a member of Parliament from Toronto, speaking by cellphone from a windowless room in the basement. \u201cI\u2019m surrounded by more than a dozen House of Commons security guards.\u201d\n\nMr. Harper had been inside Parliament at the time of the shooting but was evacuated safely, Canadian news reports said. The entire area, known as Parliament Hill, was placed on lockdown as police reinforcements arrived.\n\nThe Ottawa Police and Royal Canadian Mounted Police warned the public in a Twitter post to \u201cstay away from the downtown Ottawa area.\u201d\n\nWitnesses reported seeing the gunman who shot the soldier running into the House of Commons, firing dozens of rounds. The assailant\u2019s identity and motive were not clear.\n\nIt also was unclear whether any other people were hurt, but an Ottawa City bus converted to a medical treatment unit was seen moving to the area.\n\nJournalists covering Parliament were ordered by police officers at gunpoint to lie on the floor in the foyer in front of the House of Commons, The Globe and Mail reported on its website. The Globe and Mail\u2019s correspondent, Josh Wingrove, said in a series of Twitter posts that the hallways were filled with the smell of gunpowder.\n\nAt least 10 Royal Canadian Mounted Police squad cars converged on Parliament Hill\u2019s Centre Block, as heavily armed officers wearing bulletproof vests went into the complex.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/d9c910a3cd3f43db894216442b1d8fb7_medium.png"
          }, 
          "original": {
            "size": [
              1050, 
              591
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/d9c910a3cd3f43db894216442b1d8fb7.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/d9c910a3cd3f43db894216442b1d8fb7_thumb.png"
          }
        }, 
        "index": 38, 
        "published": 1413998079, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=on1ca1ca1&url_id=Imh0dHA6Ly93d3cubnl0aW1lcy5jb20vMjAxNC8xMC8yMy93b3JsZC9hbWVyaWNhcy9jYW5hZGEtcGFybGlhbWVudC1ndW5maXJlLmh0bWwi.HVP3CnbghXaXc1lH-kqG27p14mw&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=38", 
        "source": "http://nytimes.com/", 
        "title": "Canadian Soldier Shot in Attack at Parliament Hill in Ottawa", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=on1ca1ca1&url_id=Imh0dHA6Ly93d3cubnl0aW1lcy5jb20vMjAxNC8xMC8yMy93b3JsZC9hbWVyaWNhcy9jYW5hZGEtcGFybGlhbWVudC1ndW5maXJlLmh0bWwi.HVP3CnbghXaXc1lH-kqG27p14mw&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=38"
      }, 
      {
        "body": "Over 3 million Americans stutter, and most of us know at least one person who does. When talking to someone who stutters, interact the way you normally would. There's no need to raise your voice or avoid eye contact. Be patient, listen, and don't try to speak for the other person. The more relaxed you are, the more relaxed they will be. Keep calm and stutter on.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/94afc0617cba4c72a66fe5452ef84776_medium.png"
          }, 
          "original": {
            "size": [
              1200, 
              624
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/94afc0617cba4c72a66fe5452ef84776.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/94afc0617cba4c72a66fe5452ef84776_thumb.png"
          }
        }, 
        "index": 39, 
        "published": 1413989134, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=38&sm=1&a_id=tr1ca1ca1&url_id=.eJwVyzkOwCAMBMC_0Bv6_IZjJSyFQ7YJyu8TqqnGVbN5hbD39mvuIVZfn0cLFULP4AxipdWnoHC2mG5QWkZaodSHEVqKIlEVhTrYzvvHIa7C6BnuA5DUJgA.318waS1nFz5EcliEue51-TfPEmA&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=39", 
        "source": "http://www.upworthy.com", 
        "title": "Her Voice Is Unpredictable, But She's Not Embarrassed. Neither Is Her Audience.", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=38&a_id=tr1ca1ca1&url_id=.eJwVyzkOwCAMBMC_0Bv6_IZjJSyFQ7YJyu8TqqnGVbN5hbD39mvuIVZfn0cLFULP4AxipdWnoHC2mG5QWkZaodSHEVqKIlEVhTrYzvvHIa7C6BnuA5DUJgA.318waS1nFz5EcliEue51-TfPEmA&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=39"
      }, 
      {
        "body": "Dressing for Ebola: The 30 Steps Nurses Have to Take\nPutting on and taking off protective gear for treating an Ebola patient isn't as easy as slipping on a pair of latex gloves. It's a tedious process punctuated by liberal amounts of hand sanitizer.\nNurse Barbara Smith and Dr. Bryan Christensen demonstrated the proper way to wear and remove the full-body garb used to attend to patients suspected of being infected with Ebola. The procedure is the latest in a rapidly evolving series of protective techniques developed by the Centers for Disease Control and Prevention.\nThe new guidelines have more rigorous standards and call for a supervisor to assist in wearing, disinfecting and removing the garments. The updated guide for protective garb includes a plastic hood for covering the neck, fluid-resistant booties and an additional layer of gloves.\nIn total, there are 30 steps health care workers have to take every time they treat a patient with Ebola or Ebola-like symptoms.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/c976052a09334f73b87889e66f34b156_medium.png"
          }, 
          "original": {
            "size": [
              1200, 
              627
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/c976052a09334f73b87889e66f34b156.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/c976052a09334f73b87889e66f34b156_thumb.png"
          }
        }, 
        "index": 40, 
        "published": 1414080146, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=85&sm=1&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9tYXNoYWJsZS5jb20vMjAxNC8xMC8yMy9lYm9sYS1wcm90ZWN0aXZlLWdlYXItbnVyc2VzLyI.oy9CHO5nOZ8ujCrp7mG4WqOgSac&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=40", 
        "source": "http://mashable.com/", 
        "title": "Dressing for Ebola: The 30 Steps Nurses Have to Take", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=85&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9tYXNoYWJsZS5jb20vMjAxNC8xMC8yMy9lYm9sYS1wcm90ZWN0aXZlLWdlYXItbnVyc2VzLyI.oy9CHO5nOZ8ujCrp7mG4WqOgSac&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=40"
      }, 
      {
        "body": "Warsaw (AFP) - Poland on Thursday banned junk food in schools from January next year to trim rising rates of childhood obesity.\n\nAround 17 percent of children in Poland suffer from obesity, according to a UNICEF study published last year.\n\nLawmakers were nearly unanimous in imposing the ban, with 426 voting in favour in the 460-seat lower house of parliament.\n\nUnder the new measure, the health ministry will have to draw up a detailed list of foodstuffs approved for distribution in schools nationwide.\n\nProducts not on the list will not be allowed. Targets include potato chips, soda, burgers, candy bars and fattening processed foods.\n\nThe ban aims to \"prevent obesity and pre-obesity in children and teenagers\" a government statement said.\n\nIt was drafted by the PSL Polish Peasants' Party, the junior coalition partner in the centre-right government and representing the country's large farming sector.\n\nWorldwide obesity has nearly doubled since 1980, according to the World Health Organization.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/6c197cc0c05c4306aeaa673bcf7a22ae.png"
          }, 
          "original": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/6c197cc0c05c4306aeaa673bcf7a22ae.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/6c197cc0c05c4306aeaa673bcf7a22ae_thumb.png"
          }
        }, 
        "index": 41, 
        "published": 1414073421, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=79&sm=1&a_id=tt1to1da1&url_id=Imh0dHA6Ly9uZXdzLnlhaG9vLmNvbS9wb2xhbmQtYmFucy1qdW5rLWZvb2Qtc2Nob29scy0xODEwMjE3MzYuaHRtbCI.IxTnCZCnEPhC8-nA2fZElMyM4Pk&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=41", 
        "source": "http://news.yahoo.com/politics/", 
        "title": "Poland bans junk food in schools", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=79&a_id=tt1to1da1&url_id=Imh0dHA6Ly9uZXdzLnlhaG9vLmNvbS9wb2xhbmQtYmFucy1qdW5rLWZvb2Qtc2Nob29scy0xODEwMjE3MzYuaHRtbCI.IxTnCZCnEPhC8-nA2fZElMyM4Pk&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=41"
      }, 
      {
        "body": "Being young and healthy helped Ashoka Mukpo pull through Ebola, but he\u2019ll be weak for months, doctors who treated him said Wednesday.\n\nMukpo, a freelance journalist and camera operator who was on contract with NBC News when he got sick in Liberia, left the biocontainment unit at Nebraska Medical Center in Omaha after getting two blood tests a day apart that cleared him of the virus.\n\n\u201cAfter enduring weeks where it was unclear whether I would survive, I\u2019m walking out of the hospital on my own power, free from Ebola. This blessing is in no small measure a result of the world class care I received at the Nebraska Medical Center,\u201d Mukpo said in a statement.\n\nMukpo will also give exclusive interviews to NBC News.\n\n\u201cObviously, he has done well and we are very happy about it,\u201d said Dr. Angela Hewlett, who helped lead his treatment. \u201cWe are not sure what made him better. We are just glad he\u2019s better.\u201d\n\nMukpo, who arrived at the hospital Oct. 6, got the supportive care that\u2019s become standard in the United States \u2014 regular testing and replacement of compounds called electrolytes, which get flushed out of the body during the severe vomiting and diarrhea that mark the mid-stages of Ebola disease. The treatment is similar to what works for cholera.\n\nMukpo also got an experimental pill called brincidofovir as well as serum from Ebola survivor Dr. Kent Brantly.\n\n\u201cThank you to Dr. Kent Brantly, whose generous blood donation played a pivotal role in my recovery. May his health flourish and his compassion be known to all,\u201d Mukpo said.\n\nThe Centers for Disease Control and Prevention is testing samples of blood taken from Mukpo and other Ebola patients to see if the tests can show which treatment affects the levels of virus in the blood, but there\u2019s not much information yet, says Dr. Phil Smith, who led the treatment team.\n\nThe same team also treated medical missionary Dr. Rick Sacra, who also was infected in Liberia and was released in September. Hewlett said the team learned from that experience and made some small changes to streamline the process with Mukpo \u2014 for instance, putting a lab inside the containment zone to make it quicker to run tests and to reduce the amount of medical waste.\n\nSmith said Mukpo may be weak for several months, but he recovered more quickly than Sacra did, probably because Mukpo, 33, is 20 years young than Sacra. He\u2019ll also be vulnerable to infection. Sacra was hospitalized with pneumonia earlier this month.\n\n\u201cWith this patient gone and before we get another patient, I think we are going to use that time to share that knowledge as best we can with the rest of the world,\u201d Smith said.\n\nIt\u2019s a labor-intensive effort to take care of a patient with Ebola. Several separate rooms were designated for suiting up, running lab tests and taking off the personal protective equipment needed to keep doctors, nurses and technicians from getting infected.\n\nSmith estimates that, at any given time, 10 people can be on duty taking care of an Ebola patient. At least one caregiver such as a nurse is in the room with the patient at all times, and someone is always posted in the hallway to make sure protective gear gets taken off correctly.\n\nLinens and other materials are decontaminated at high temperatures in an autoclave before they leave the facility, and all staff involved in Mukpo\u2019s care will monitor their temperatures for 21 days.\n\nMukpo asked people to think of people in Liberia, Sierra Leone and Guinea, where the World Health Organization now says nearly 10,000 people have been infected and 4,800 have died.\n\n\u201cI saw many haunting images in Liberia that I will carry through my life. Nobody deserves to die under the circumstances that have existed in West Africa since this outbreak began,\u201d Mukpo said.\n\n\u201cI hope our global community will ramp up its efforts to curtail the epidemic but also to save the lives of the sick. I know firsthand that this disease is treatable and hope that some approximation of the care I received can be given to sick Africans. My prayers are with the Liberian, Sierra Leonean, and Guinean people.\u201d", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/71e46715a839463bac40b841f7a5e453_medium.png"
          }, 
          "original": {
            "size": [
              2500, 
              1667
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/71e46715a839463bac40b841f7a5e453.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/71e46715a839463bac40b841f7a5e453_thumb.png"
          }
        }, 
        "index": 42, 
        "published": 1414000273, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=39&sm=1&a_id=ttmv1tv1so1&url_id=.eJwlzGEOwiAMBtC77P83Mk2M8TYFqxBYuxQY4fZqPMB7S2zteDg3xljFB-FR16C7q01tliTs2GshnMl6hfbmjSm7qV3eiEylxYmoA1-Mn8bLmAtJYAPVqJmw93woarcznfzEP5TLdbvdt-UDbUkv7w.AA53wbhB4LcjbQeXDyZ2sdmX3_I&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=42", 
        "source": "http://nbcnews.com/", 
        "title": "Young and Healthy: How NBC News Freelancer Survived Ebola", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=39&a_id=ttmv1tv1so1&url_id=.eJwlzGEOwiAMBtC77P83Mk2M8TYFqxBYuxQY4fZqPMB7S2zteDg3xljFB-FR16C7q01tliTs2GshnMl6hfbmjSm7qV3eiEylxYmoA1-Mn8bLmAtJYAPVqJmw93woarcznfzEP5TLdbvdt-UDbUkv7w.AA53wbhB4LcjbQeXDyZ2sdmX3_I&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=42"
      }, 
      {
        "body": "In the lead-up to the midterms, President Barack Obama has been parroting the conventional wisdom about the GOP\u2019s future: Republicans are doomed if they keep up their opposition to immigration reform and continue the inflammatory anti-immigrant rhetoric. \u201cIt\u2019s anybody\u2019s guess how Republicans are thinking about this,\u201d he said during a town hall event in Santa Monica, California. \u201cIf they were thinking long term politically, it is suicide for them not to do this.\u201d Latinos make up 14 percent of the population, and their share is projected to grow to 29 percent by 2050. This demographic traditionally identifies with the Democratic Party; the toxic immigration debate in Washington, fueled by xenophobes in the GOP, will only increase that tendency. In 2006, 49 percent of Latino eligible voters identified as or leaned Democratic. By 2011, that number jumped to 67 percent. With the United States projected to become a majority-minority country by 2043, Republicans\u2019 chances of winning the White House on the backs of white voters will grow ever slimmer. But a counternarrative, one that would put Latino votes back in contention for the GOP, has begun to emerge. In the coming decades, Latinos could become \u201cwhite\u201d \u2014 a process in which cultural assimilation would presumably be followed by political realignment \u2014 opening them up to affiliation with the Republican Party. It\u2019s a theory espoused most prominently by Slate political writer Jamelle Bouie, who argues in the winter issue of Democracy that \u201cthe future won\u2019t be majority-minority; it will be a white majority, where Spanish last names are common.\u201d But this vision of complete assimilation ignores the stark racial divisions in Latin American societies, in which socioeconomic status and skin color, as in the U.S., tend to fall along parallel lines.\n\nThe idea of Latinos becoming white in the American sense \u2014 a vision of racial and cultural assimilation independent of self-identified race \u2014 isn\u2019t a new one. Economists Brian Duncan at the University of Colorado and Stephen Trejo at the University of Texas at Austin call it ethnic attrition. As Latinos intermarry and climb the socioeconomic ladder, the theory goes, they are less likely to self-identify as Hispanic. Duncan and Trejo\u2019s research shows (PDF) that while virtually all first- and second-generation Hispanic immigrants identify as Hispanic, in the third generation, those of mixed heritage start to self-select out of this group. Among third-generation immigrants with only two Hispanic grandparents, 79 percent identify as Hispanic. Among those with only one Hispanic grandparent, the number falls to 58 percent. Think of Republican Sen. Ted Cruz, whose father is Cuban and whose mother is white, or comedian Louis C.K., whose grandmother is Mexican and whose other grandparents are Irish and Hungarian. Racial self-identification tends to be reflected in one\u2019s politics. A recent analysis of election-survey data by Spencer Piston, a political scientist at Syracuse University, shows that lighter-skinned Latinos, who are more likely to identify as white, vote Republican at higher rates than those with darker skin. Bouie\u2019s prediction is that in the future, more and more Latinos will identify as white and that a substantial number of them will also identify as Republicans. Democrats\u2019 dreams of a solid future majority could thus be imperiled. History shows just how fluid such self-identification is. As historian Noel Ignatiev argues in his landmark work, \u201cHow the Irish Became White,\u201d when Irish immigrants arrived in the United States in the 1800s, they faced significant discrimination at the hands of the Anglo-American ruling class. Irish-Americans were for generations a reliable Democratic voting bloc, but intermarriage and the Democratic Party\u2019s embrace of African-American rights led to a political realignment. Irish-Americans came to view themselves \u2014 and be viewed \u2014 as part of the white mainstream. While these voters continued to lean Democratic, by the 1980s they joined the coalition that elected Ronald Reagan to the presidency.\n\nWill Latinos follow the patterns of Irish immigrants before them? To an extent, certainly. One of the strongest pieces of evidence for this \u2014 and the reason Latinos are the group commentators most frequently talk about becoming \u201cwhite\u201d \u2014 is that interracial marriage rates are highest between whites and Hispanics. A full 80 percent of third-generation Mexican-Americans are the product of intermarriage. Another finding that has fueled much of the recent discussion about Latino self-identification is a study from the Pew Research Center earlier this year showing that 2.5 million Americans changed their self-identified race and ethnicity from \u201cHispanic and some other race\u201d in the 2000 census to \u201cHispanic white\u201d in the 2010 census. But as Julio Varela at the blog Latino Rebels suggests, the 2.5 million Latinos who switched their identity from just \u201cHispanic\u201d to \u201cHispanic white\u201d most likely reflects confusion or ambivalence about how to label oneself rather than a realignment of racial identity. Case in point: The same study of census data showed that 1.3 million Latinos made the switch in the opposite direction.\n\nBy assuming uniform motivations, the \u201ctoday\u2019s Latinos, tomorrow\u2019s whites\u201d framework also flattens a racially diverse group \u2014 one that includes light-skinned people whose ancestors hail from Spain; indigenous South Americans; blacks in the Caribbean, Brazil and Colombia with roots in Africa; Asian immigrants to Latin America; and those with mixed European and indigenous heritage. Immigrants hailing from the 20 countries south of the U.S. border, tend to share certain characteristics. Reflecting a history of colonization, they tend to speak Spanish or Portuguese and practice Catholicism; their families tend to be bigger; Latin American cultures tend to be more collectivist. In the U.S., attacks on immigrants have increasingly made those with roots in Mexico and Central and South America see their political fates as intertwined. But if asked, most Latinos in the U.S. refer to themselves by their national-origin group \u2014 Mexican, Puerto Rican, Cuban. And while it doesn\u2019t look like immigration reform is passing any time soon, if it does, Latinos may be even less likely to use the pan-ethnic Latino label. This isn\u2019t to say that light-skinned Latinos of European descent won\u2019t increasingly assimilate into the white mainstream as Irish (and Italian) immigrants did. That\u2019s already happening, to an extent. But whether this will be the case with other subgroups is an open question, in part because there isn\u2019t much data on it. Because of the persistence of the United States\u2019 limited black/white/Asian/Latino classification system, we don\u2019t know the intermarriage rates between black Hispanics and whites or whites and Hispanics of indigenous descent. Nor do we know the racial composition of Hispanics who checked \u2014 or did not check \u2014 the \u201cwhite\u201d box in the 2010 census. Finally, a simple but important factor that often gets overlooked in discussions about Latino racial identity is the persistence of discrimination, which tends to strengthen existing racial categories. (Remember that even highly successful mixed blacks such as the president continue to face discrimination, and while Obama jokes about standing out as white among blacks, most of the American public considers him black.) To ask whether Latinos will see themselves as Latino or white in the future is also to ask how long the GOP will continue to be dominated by the likes of Iowa Rep. Steve King, who said that for every undocumented minor who becomes a valedictorian, \u201cthere\u2019s another hundred out there who weigh 130 pounds \u2014 and they\u2019ve got calves the size of cantaloupes because they\u2019re hauling 75 pounds of marijuana across the desert.\u201d", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/d11a2d1a46c646f8aacb45381b6dbefa_medium.png"
          }, 
          "original": {
            "size": [
              1460, 
              913
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/d11a2d1a46c646f8aacb45381b6dbefa.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/d11a2d1a46c646f8aacb45381b6dbefa_thumb.png"
          }
        }, 
        "index": 43, 
        "published": 1414029610, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=34&sm=1&a_id=tr1ca1ca1&url_id=.eJwNyzEOgCAMAMC_uEPROPmbShpbAy2BJkRfr_vdwu7tAMBKXTJGLDe-RB1jtgrWRMV0wJbWHdYEk59Q0EVthGka_KTf0WTx_2QiZ5Us_lzWInstywesYiPO.-BvLXZF3qIP47hm_ZkALEUGqNCc&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=43", 
        "source": "http://digg.com/", 
        "title": "Why Latinos Won't Become White", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=34&a_id=tr1ca1ca1&url_id=.eJwNyzEOgCAMAMC_uEPROPmbShpbAy2BJkRfr_vdwu7tAMBKXTJGLDe-RB1jtgrWRMV0wJbWHdYEk59Q0EVthGka_KTf0WTx_2QiZ5Us_lzWInstywesYiPO.-BvLXZF3qIP47hm_ZkALEUGqNCc&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=43"
      }, 
      {
        "body": "US-led airstrikes have killed 553 Islamist militants and 32 civilians in Syria during a month-long campaign, a monitoring group has said.\n\nMost of those killed - 464 - were Islamic State fighters, the Britain-based Syrian Observatory for Human Rights said. Fifty-seven were from al Qaeda-linked al Nusra Front.\n\nSix children and five women were among the civilians killed, said the Observatory, which relies on a network of activists around Syria.\n\nUS Central Command spokesman Colonel Patrick Ryder earlier said Washington takes \"reports of civilian casualties or damage to civilian facilities seriously and we have a process to investigate each allegation\".\n\nThe coalition strikes have bombed the Syrian provinces of Aleppo, Deir al Zor, Idlib, Raqqa and al Hassakah, the Observatory said.\n\nIn the Aleppo district, the town of Kobani, on the Turkish border, has become a crucial battleground in the IS fight.\n\nKurdish forces have been defending the besieged town against the militants, who have been making significant gains despite the US-led forces hitting their positions.\n\nBut the Kurds have managed to halt the IS advance and held most of the key town, the US military has said.\n\nThe Kurdish fighters have been boosted by Iraqi Kurdish politicians agreeing to send much-needed reinforcements and US weapons airdrops.\n\nBut two of the arms bundles intended for the Kurds went astray earlier this week, the Pentagon said. One was destroyed in a strike and the other fell into the hands of IS fighters.\n\nIS released a video online, allegedly shot in Kobani, showing its fighters going through boxes containing hand grenades and rocket-propelled grenades.\n\nIslamic State has already grabbed large parts of Syria and neighbouring Iraq. With the help of Arab allies, the US has been carrying out airstrikes in Iraq against IS since July and in Syria since September.\n\nThe UK and France have also struck IS targets in Iraq.\n\nEarlier this week, Britain's Defence Secretary Michael Fallon announced RAF Reaper drones would be flying surveillance missions over Syria to gather intelligence on IS.\n\nBut the use of weapons has not been authorised and the British Government has insisted that strike missions in the country would only be carried out with parliamentary approval.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/4318e886b5194c538602b8ef3eed3874_medium.png"
          }, 
          "original": {
            "size": [
              1600, 
              900
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/4318e886b5194c538602b8ef3eed3874.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/4318e886b5194c538602b8ef3eed3874_thumb.png"
          }
        }, 
        "index": 44, 
        "published": 1414060375, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=83&sm=1&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9uZXdzLnNreS5jb20vc3RvcnkvMTM1ODY4MS91cy1sZWQtYWlyc3RyaWtlcy1hZ2FpbnN0LWlzLWluLXN5cmlhLWtpbGwtNTUzIg.URb6K4q9qPJpb_Vn5VGoaW1IM9M&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=44", 
        "source": "http://news.sky.com/", 
        "title": "US-Led Airstrikes Against IS In Syria Kill 553", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=83&a_id=ve1ve1de1&url_id=Imh0dHA6Ly9uZXdzLnNreS5jb20vc3RvcnkvMTM1ODY4MS91cy1sZWQtYWlyc3RyaWtlcy1hZ2FpbnN0LWlzLWluLXN5cmlhLWtpbGwtNTUzIg.URb6K4q9qPJpb_Vn5VGoaW1IM9M&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=44"
      }, 
      {
        "body": "Scientists routinely study deadly pathogens like Ebola in order to find ways to fight them and discover potential cures. But what would happen if a sample of Ebola was taken from a lab illegally?\n\nUnder federal regulations, Ebola is considered a \u201cselect agent and toxin\u201d that has the \u201cpotential to pose a severe threat to public health and safety,\u201d and it\u2019s illegal to possess, use or transfer a deadly pathogen to another individual without a certificate from the U.S. Department of Health and Human Services, says John Kraemer, an expert on infectious diseases and the law at Georgetown University\u2019s Department of Health Systems Administration. Obtaining that certificate requires meeting a set of biosafety and biosecurity requirements. And the penalties for failing to do so can be steep.\n\nThe government has levied fines of hundreds of thousands of dollars to laboratories that have violated the select agent regulations. In 2008, HHS docked Texas A&M University $1 million for safety violations at its biodefense lab. Individuals who steal a disease sample could face similarly steep fines and time behind bars. Under federal law, HHS can fine a person up to $250,000 for each violation and can recommend imprisonment of up to five years.\n\nBut there is an additional layer of sensitivity to handling Ebola. The CDC considers viral hemorrhagic fevers, which includes Ebola, a Category A bioterrorism agent. And since 2001, several bioterrorism laws have strengthened criminal penalties against those who attempt to commandeer them. The Patriot Act in 2001 created a provision banning the transfer of a select agent like Ebola, and the Bioterrorism Act of 2002 gave more authority to the HHS to regulate those agents and diseases.\n\nIn September, the Obama administration issued new regulations for federally funded labs that work with contagious diseases like Ebola. Some researchers have criticized the guidelines as not being strong enough over fears that the pathogens, which are often made stronger in a lab, could potentially be used as bioweapons.\n\nKraemer says two scenarios could likely play out if Ebola samples fell into the wrong hands. If a researcher acquired Ebola for misguided research, for example, then they would likely get fined by HHS and could be sentenced to five years in prison.\n\n\u201cIf however someone broke into a hospital to steal Ebola for some other reason, it\u2019d be at least 10 years,\u201d Kraemer says. \u201cIf someone acquires Ebola with an intent to weaponize it, then they can get life in prison. And, of course, if you actually use Ebola as a weapon, you can be prosecuted under federal anti-terrorism laws, with penalties up to the death penalty.\u201d\n\nGiven the security required at labs authorized to handle potential biological weapons, as well as the risk that someone stealing a pathogen may also become infected by it, those latter scenarios are highly unlikely.\n\n\u201cStealing an Ebola sample would be extremely dangerous because the thief would face a significant risk of exposure,\u201d says Robert Field, a professor of law at Drexel University. \u201cOther pathogens would be safer to steal because protection is easier.\u201d", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/abfdeec2207942a39d3f8b4c1241eb62_medium.png"
          }, 
          "original": {
            "size": [
              1012, 
              760
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/abfdeec2207942a39d3f8b4c1241eb62.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141122/abfdeec2207942a39d3f8b4c1241eb62_thumb.png"
          }
        }, 
        "index": 45, 
        "published": 1414027147, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=85&sm=1&a_id=ve1ve1de1&url_id=Imh0dHA6Ly90aW1lLmNvbS8zNTMyMDU3L2Vib2xhLWJpb3dlYXBvbi10ZXJyb3Jpc20vIg.imEhkfRHRohI0Vn2j-F1gO70o1Q&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=45", 
        "source": "http://time.com/", 
        "title": "Here\u2019s What Would Happen if Ebola Was Stolen From a Lab", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=85&a_id=ve1ve1de1&url_id=Imh0dHA6Ly90aW1lLmNvbS8zNTMyMDU3L2Vib2xhLWJpb3dlYXBvbi10ZXJyb3Jpc20vIg.imEhkfRHRohI0Vn2j-F1gO70o1Q&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=45"
      }, 
      {
        "body": "Abandon all hope, all ye who enter here. This is the first look at Disney's Into the Woods Big Bad Wolf, and that is definitely Johnny Depp in a zoot suit with wolf ears. YIKES. Everyone else looks great, though.\nEntertainment Weekly has just unleashed four Into The Woods movie preview covers, thus revealing the official look of Into the Wood's Big Bad Wolf. And he looks like a wolf from a Tex Avery cartoon.\nYep, that's Johnny Depp, who appears to be channeling someone from the Cherry Poppin' Daddies crossed with the cartoon character wolf from the 1943 \"Red Hot Riding Hood\" cartoon. He's even got a wallet chain! The reason Depp's lothario-wolf look is so creepy is because Disney has cast the extremely young Lilla Crawford as Red Riding Hood. In the original musical, the original Red was played by 16-year-old Danielle Ferland, which fit in well with the show's \"loss of innocence\" themes that surround the character. The Big Bad Wolf even had a giant penis attached to his costume in the musical, so it's not like it was subtle.\nBut Lilla Crawford is 13 or 14 now (back in 2012 Huff Po reported that she was 11-years-old), which is a big difference from 16. So why is Johnny Depp's Wolf still looking like a sexual predator? It's weird and kind of icky. Thank goodness Disney didn't go with their first choice for Red, Sophia Grace \u2014 she's even younger than Crawford.\nWhy channel a dated lothario look at all? This doesn't even work with the rest of the Renaissance costumes. Does this mean that Disney IS going to have Depp seduce a young child? I highly, highly doubt it. But this most likely means that Red's solo \"I Know Things Now\" is probably very different, or was scrapped entirely. Then again if I was going to cast anyone to make a live action version of \"Red Hot Riding Hood\" I would choose Deep, and an older woman. So I'm torn, because I think the suit is hilarious. But does it work for Into The Woods and I'm 100% happy we are spared the exposed abs outfit from the original musical. But does this version work?", 
        "images": {
          "medium": {
            "size": [
              500, 
              338
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/5c8f9110b78144e5b987f968819f14b4_medium.png"
          }, 
          "original": {
            "size": [
              667, 
              452
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/5c8f9110b78144e5b987f968819f14b4.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/5c8f9110b78144e5b987f968819f14b4_thumb.png"
          }
        }, 
        "index": 46, 
        "published": 1413992520, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=33&sm=1&a_id=tr1ca1ca1&url_id=.eJwlyU0OgjAQQOGrEBZGY8ZqIERIiDsXXsK0dArFttP0JwZPL-Lyfa-cUvIdY5ra00CWzTQ5t4BE7yMIPYLgEt5kFKhAFqSODpcI2iWCNOG6SK4Jl6Zuq-rcXGt2fPGEMmiMt5zsM1IOA_YKUYocHIbdTy1Kne2mWw_ceq5H199X6YoZPyjQMJWNKfaPfx3KL0UaPo0.Krde-stAz_D8fniCRhu3SDIQ-tc&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=46", 
        "source": "http://jezebel.com/", 
        "title": "Johnny Depp's Big Bad Wolf From Disney's Into The Woods Is Just Bad", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=33&a_id=tr1ca1ca1&url_id=.eJwlyU0OgjAQQOGrEBZGY8ZqIERIiDsXXsK0dArFttP0JwZPL-Lyfa-cUvIdY5ra00CWzTQ5t4BE7yMIPYLgEt5kFKhAFqSODpcI2iWCNOG6SK4Jl6Zuq-rcXGt2fPGEMmiMt5zsM1IOA_YKUYocHIbdTy1Kne2mWw_ceq5H199X6YoZPyjQMJWNKfaPfx3KL0UaPo0.Krde-stAz_D8fniCRhu3SDIQ-tc&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=46"
      }, 
      {
        "body": "The new Gmail app from the Gmail team isn't technically just an email app, at least if you ask them. It's called \"Inbox,\" and it's being released as an invite-only system that works on the web, Android phones, and iPhones. It feels completely native and fast on all of those systems. But it's a native and fast app that does something 10 degrees away from what you'd expect an email app to do. My first impression of Inbox is that it's really great, but a little weird.\n\nThe basic idea is this: it's still a Gmail app, but instead of giving you the traditional list of emails, it tries to intelligently give you more information so you don't have to even open them. Google Now-style info cards appear right in line with your message list, including things like flight times, package tracking, and photos.\n\nIt also tries to intelligently \"bundle\" emails into groups that you can quickly dismiss. So instead of having those annoying category tabs in Gmail, you have all your promotions and whatnot collapsed down into a single line in your Inbox. You can drill in and \"pin\" the ones you want to save and then dismiss the rest. Google is also applying its algorithms to automatically parse out things like phone numbers and addresses when you need them.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/265f38aaf6844160b366089778f7f817_medium.png"
          }, 
          "original": {
            "size": [
              1200, 
              675
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/265f38aaf6844160b366089778f7f817.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/265f38aaf6844160b366089778f7f817_thumb.png"
          }
        }, 
        "index": 47, 
        "published": 1413982801, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&sm=1&a_id=on1ca1ca1&url_id=Imh0dHA6Ly93d3cudGhldmVyZ2UuY29tLzIwMTQvMTAvMjIvNzAzOTM5MS9nb29nbGUtaW5ib3gi.r11pB0Pwvs7rBdIuMiEE5g0muHg&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=47", 
        "source": "http://theverge.com/", 
        "title": "Inbox is a total reinvention of email from Google", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=100&a_id=on1ca1ca1&url_id=Imh0dHA6Ly93d3cudGhldmVyZ2UuY29tLzIwMTQvMTAvMjIvNzAzOTM5MS9nb29nbGUtaW5ib3gi.r11pB0Pwvs7rBdIuMiEE5g0muHg&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=47"
      }, 
      {
        "body": "Counter-terrorism officers trying to staunch the flow of recruits travelling to Syria have made two arrests they say may be linked to the war zone.\n\nA woman aged 25 was arrested in Kempston, Bedfordshire by detectives from Scotland Yard\u2019s counter-terrorism command investigating whether she had travelled to Syria, and if so, whether that trip was linked to violent jihad.\n\nHours later officers made a second arrest in London, detaining a 32-year-old man \u201con suspicion of attending a place used for terrorist training\u201d, which they believe was in Syria.\n\nThe two operations that led to the arrests are not believed to be linked.\n\nOn Tuesday, the Metropolitan police commissioner, Sir Bernard Hogan-Howe, said five Britons a week were travelling to Syria to join up with Islamic State (Isis) extremists.\n\nCounter-terror officials say there has been a large increase this year in operations related to Syria, amid fears that returning Britons may be so radicalised they attempt to carry out attacks here.\n\nIn the first arrest, police said the woman was arrested in Bedfordshire \u201con suspicion of preparation of terrorist acts\u201d. After the 25-year-old was detained, police searched two addresses in Bedfordshire as part of their inquiries.\n\nIn the second arrest, the man aged 32 was detained at an address in south-west London. Police were searching an address in south-west London and another in west London as part of their investigation.\n\nPolice said both investigations were Syria related.\n\nBoth of those arrested were in police custody in central London where they are expected to be interviewed.\n\nOn Tuesday Hogan-Howe said the \u201cdrumbeat of terrorism in the UK\u201d was now \u201cfaster and more intense\u201d.\n\nHe said 500 Britons were believed to have travelled to Syria: \u201cThose are the ones that we believe have gone. There may be many more who set out to travel to another country and meandered over to Syria and Iraq in a way that is not always possible to spot when you have failed states and leaky borders.\u201d\n\nLast week police said there had been 218 terror-related arrests so far this year, a significant increase, as a result of police \u201crunning exceptionally high numbers of counter-terrorism investigations\u201d.\n\nThey added that this year, 16 people have been charged after returning from Syria.", 
        "images": {
          "medium": {
            "size": [
              500, 
              500
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/c5781fad66314a40ae4f2622d515c288_medium.png"
          }, 
          "original": {
            "size": [
              2560, 
              1536
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/c5781fad66314a40ae4f2622d515c288.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141121/c5781fad66314a40ae4f2622d515c288_thumb.png"
          }
        }, 
        "index": 48, 
        "published": 1413992777, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=83&sm=1&a_id=ve1ve1de1&url_id=.eJwNyUkOgDAIAMC_eEe08eRvsBKLG03BEH-vc52uuNcZMSJ6L7w91Fahu8964XPAzWGYhnFCzY4pYdVTMsNf1Bqbg4dCVTNZToZdCq1gbxPqPqewIC0.U10uC9C9Lhj2NDwDpQtVRK1K0mA&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=48", 
        "source": "http://observer.guardian.co.uk/", 
        "title": "Police in UK arrest two over possible links to jihad in Syria", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=83&a_id=ve1ve1de1&url_id=.eJwNyUkOgDAIAMC_eEe08eRvsBKLG03BEH-vc52uuNcZMSJ6L7w91Fahu8964XPAzWGYhnFCzY4pYdVTMsNf1Bqbg4dCVTNZToZdCq1gbxPqPqewIC0.U10uC9C9Lhj2NDwDpQtVRK1K0mA&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=48"
      }, 
      {
        "body": "As President Barack Obama noted in his weekly address Saturday, Ebola is a serious public health issue. But the level of paranoia that has surfaced across the country since Thomas Duncan became the first patient diagnosed with the disease in the United States is not only unwarranted\u2014it's  dangerous. Ripped straight from the headlines, here are just five of the more surreal incidents of Ebola panic.\n\nSyracuse University disinvites photographer. Ebola has an incubation period of up to three weeks. If someone hasn't gotten sick within 21 days of exposure, they're in the clear. But News Photographer magazine reported last week that \"three-time Pulitzer Prize-winning photojournalist Michel du Cille of The Washington Post, who returned from covering the Ebola crisis in Liberia 21 days ago and who is symptom free, was asked by Syracuse University officials today not to come to campus, where he was scheduled to participate in a journalism program.\" Cille was not pleased:\n\nMaine teacher put on leave after traveling to Dallas. \"A teacher at Strong Elementary School was placed on a 21-day paid leave of absence after parents told the school board they were concerned that she might have been exposed to Ebola during a trip to Dallas for an educational conference,\" the Portland Press Herald recently reported. Dallas, where Duncan's case was first diagnosed, is a city of 1.25 million. Five million people travel to and from Dallas every month.\n\nRwandan students kept home from New Jersey elementary school. Two students who moved from Rwanda\u2014where there have been zero cases of Ebola\u2014are being kept home from school in Burlington County, N.J. for 21 days in response to concerns from parents. Rwanda \"is about 2600 miles away from the closest affected country in West Africa,\" notes Philadelphia's local Fox station. \"That's about as close as Seattle, Washington is to Philadelphia. But for some parents it really doesn't matter.\"\n\nCleveland man charged with felony after stupid joke. \"Bond is set at $10,000 for a Cleveland man charged with inducing panic after being accused of telling a Horseshoe Casino worker that he was gambling to avoid his Ebola-stricken ex-wife,\" Cleveland.com reported last week. Needless to say, neither the man nor his wife have Ebola.\n\nTexas college rejects applicants from Ebola-free Nigeria. Officials at Navarro College in Texas cited Ebola as a basis for refusing admission to two Nigerian students. Nigeria has been extraordinarily effective in fighting its recent outbreak, which  included just 20 confirmed cases\u2014so extraordinary, in fact, that as of today, the World's Health Organization officially declared the country Ebola free. After the media caught wind of the story, an official from Navarro pushed back against \"misinformation\" by saying that the college is focusing on students from China and Indonesia for the next year.\n\nThere's much, much more out there, but we leave you with this note from Bloomberg's Gabriel Snyder.", 
        "images": {
          "medium": {
            "size": [
              500, 
              280
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141219/75f630e3f5114d93b0c7ec8d3834cb55_medium.png"
          }, 
          "original": {
            "size": [
              630, 
              354
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141219/75f630e3f5114d93b0c7ec8d3834cb55.png"
          }, 
          "thumbnail": {
            "size": [
              200, 
              200
            ], 
            "url": "https://swayycontent.s3.amazonaws.com/images/20141219/75f630e3f5114d93b0c7ec8d3834cb55_thumb.png"
          }
        }, 
        "index": 49, 
        "published": 1413837716, 
        "share_url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=44&sm=1&a_id=ttmv1tv1so1&url_id=Imh0dHA6Ly93d3cubW90aGVyam9uZXMuY29tL21vam8vMjAxNC8xMC9lYm9sYS1hbWVyaWNhLXBhbmljLWh5c3RlcmlhIg.QASEkTcFv5gX9-2reD3KGJ8DBGk&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=49", 
        "source": "http://motherjones.com/", 
        "title": "The 5 Stupidest Paranoid Responses to Ebola", 
        "url": "http://feed.swayy.co/?partner_id=sendible-test&a_s=44&a_id=ttmv1tv1so1&url_id=Imh0dHA6Ly93d3cubW90aGVyam9uZXMuY29tL21vam8vMjAxNC8xMC9lYm9sYS1hbWVyaWNhLXBhbmljLWh5c3RlcmlhIg.QASEkTcFv5gX9-2reD3KGJ8DBGk&feed_id=6ebda66db178427ca6a3581c1ca14cb5_50&i=49"
      }
    ]
  }
}

```