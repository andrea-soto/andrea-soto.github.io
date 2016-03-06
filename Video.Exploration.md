
# Facebook

### [Facebook Graph Explorer](https://developers.facebook.com/tools/explorer/145634995501895/?method=GET&path=%7Bpage-id%7D&version=v2.5)

**Help and Resources:**

- Getting page access tokens [link](http://aseriesoftubes.com/articles/obtaining-facebook-page-access-tokens-the-4-step-program/)

## Sample Requests

`me?fields=id,name,photos`

`MarsCuriosity/videos`

`HuffingtonPost/videos`

`MarsCuriosity?fields=videos.limit(1){id,likes.limit(1).summary(1)}`

`HuffingtonPost?fields=videos.limit(1){id,likes.limit(0).summary(1),comments.limit(0).summary(1)}`

`HuffingtonPost?fields=posts.limit(40){likes.limit(1).summary(1),comments.limit(1).summary(1)}`


### **Fields have to be explicitly requested, or WILL NOT be returned in response!**


## Sample Video

See [video](https://www.facebook.com/HuffingtonPost/videos/10153717150501130/)

**Thumbnails**

`HuffingtonPost?fields=videos.limit(2){id,thumbnails}`

``` javascript
"thumbnails":  
  { "data": [ 
    { "id": "10153717151076130",
      "height": 720,
      "scale": 1,
      "uri": "https://scontent.xx.f..."
    }
  ]}
``` 

See [Thumbnail](https://scontent.xx.fbcdn.net/hvthumb-xtf1/v/t15.0-10/12419394_10153717151086130_1619157744_n.jpg?oh=cfbfdfaea1914f4a65ff402df3a9fd35&oe=575CC4BE)

# NEXT: Find video in Twitter 

See video at: http://pbs.twimg.com/ext_tw_video_thumb/700760287205437440/pu/img/tvpaZCnohqwYcONH.jpg

### [Twitter Console](https://dev.twitter.com/rest/tools/console)

**Help and Resources:**

- How to Explore Twitter API [link](https://mashe.hawksey.info/2015/04/how-to-explore-the-twitter-api-without-code-using-the-console-2/)

**Thumbnails**

``` javascript
"entities":  
    { "media": [  
          { "id": 700760287205437400, 
            "media_url": "http://pbs.twimg.com/ext_tw_video_thumb/700760..." }  
 ] }
```

See [Thumbnail](https://twitter.com/search?f=videos&vertical=default&q=cheese%20italian%20dip&src=typd)







---

## Twitter JSON Object

``` javascript
{
  "created_at": "Fri Feb 19 19:15:37 +0000 2016",
  "id": 700760666336931800,
  "id_str": "700760666336931840",
  "text": "3 Cheese Italian Dip & Chips https://t.co/HnKs7EkPza",
  "truncated": false,
  "source": "<a href="http://twitter.com" rel="nofollow">Twitter Web Client</a>",
  "in_reply_to_status_id": null,
  "in_reply_to_status_id_str": null,
  "in_reply_to_user_id": null,
  "in_reply_to_user_id_str": null,
  "in_reply_to_screen_name": null,
  "user":  {
    "id": 16402507,
    "id_str": "16402507",
    "name": "Thrillist",
    "screen_name": "Thrillist",
    "location": "",
    "description": "The essential resource for how to spend your time and money. Now go be awesome. Add us on Snapchat: https://t.co/ZoLC91CPS5",
    "url": "https://t.co/JTS9L78iqU",
    "entities":  {
      "url":  {
        "urls":  [
           {
            "url": "https://t.co/JTS9L78iqU",
            "expanded_url": "http://www.thrillist.com",
            "display_url": "thrillist.com",
            "indices":  [
              0,
              23
            ]
          }
        ]
      },
      "description":  {
        "urls":  [
           {
            "url": "https://t.co/ZoLC91CPS5",
            "expanded_url": "http://bit.ly/1VqdWyp",
            "display_url": "bit.ly/1VqdWyp",
            "indices":  [
              100,
              123
            ]
          }
        ]
      }
    },
    "protected": false,
    "followers_count": 98946,
    "friends_count": 3772,
    "listed_count": 2521,
    "created_at": "Mon Sep 22 12:19:06 +0000 2008",
    "favourites_count": 10320,
    "utc_offset": -18000,
    "time_zone": "Eastern Time (US & Canada)",
    "geo_enabled": true,
    "verified": true,
    "statuses_count": 23828,
    "lang": "en",
    "contributors_enabled": false,
    "is_translator": false,
    "is_translation_enabled": false,
    "profile_background_color": "808080",
    "profile_background_image_url": "http://pbs.twimg.com/profile_background_images/440916519824814080/zoaE9KLH.jpeg",
    "profile_background_image_url_https": "https://pbs.twimg.com/profile_background_images/440916519824814080/zoaE9KLH.jpeg",
    "profile_background_tile": true,
    "profile_image_url": "http://pbs.twimg.com/profile_images/678681815964610560/bIoP0rSU_normal.jpg",
    "profile_image_url_https": "https://pbs.twimg.com/profile_images/678681815964610560/bIoP0rSU_normal.jpg",
    "profile_banner_url": "https://pbs.twimg.com/profile_banners/16402507/1415133761",
    "profile_link_color": "0084B4",
    "profile_sidebar_border_color": "FFFFFF",
    "profile_sidebar_fill_color": "FFFFFF",
    "profile_text_color": "333333",
    "profile_use_background_image": true,
    "has_extended_profile": false,
    "default_profile": false,
    "default_profile_image": false,
    "following": false,
    "follow_request_sent": false,
    "notifications": false
  },
  "geo": null,
  "coordinates": null,
  "place": null,
  "contributors": null,
  "is_quote_status": false,
  "retweet_count": 5,
  "favorite_count": 16,
  "entities":  {
    "hashtags":  [],
    "symbols":  [],
    "user_mentions":  [],
    "urls":  [],
    "media":  [
       {
        "id": 700760287205437400,
        "id_str": "700760287205437440",
        "indices":  [
          33,
          56
        ],
        "media_url": "http://pbs.twimg.com/ext_tw_video_thumb/700760287205437440/pu/img/tvpaZCnohqwYcONH.jpg",
        "media_url_https": "https://pbs.twimg.com/ext_tw_video_thumb/700760287205437440/pu/img/tvpaZCnohqwYcONH.jpg",
        "url": "https://t.co/HnKs7EkPza",
        "display_url": "pic.twitter.com/HnKs7EkPza",
        "expanded_url": "http://twitter.com/Thrillist/status/700760666336931840/video/1",
        "type": "photo",
        "sizes":  {
          "small":  {
            "w": 340,
            "h": 340,
            "resize": "fit"
          },
          "thumb":  {
            "w": 150,
            "h": 150,
            "resize": "crop"
          },
          "medium":  {
            "w": 600,
            "h": 600,
            "resize": "fit"
          },
          "large":  {
            "w": 720,
            "h": 720,
            "resize": "fit"
          }
        }
      }
    ]
  },
  "extended_entities":  {
    "media":  [
       {
        "id": 700760287205437400,
        "id_str": "700760287205437440",
        "indices":  [
          33,
          56
        ],
        "media_url": "http://pbs.twimg.com/ext_tw_video_thumb/700760287205437440/pu/img/tvpaZCnohqwYcONH.jpg",
        "media_url_https": "https://pbs.twimg.com/ext_tw_video_thumb/700760287205437440/pu/img/tvpaZCnohqwYcONH.jpg",
        "url": "https://t.co/HnKs7EkPza",
        "display_url": "pic.twitter.com/HnKs7EkPza",
        "expanded_url": "http://twitter.com/Thrillist/status/700760666336931840/video/1",
        "type": "video",
        "sizes":  {
          "small":  {
            "w": 340,
            "h": 340,
            "resize": "fit"
          },
          "thumb":  {
            "w": 150,
            "h": 150,
            "resize": "crop"
          },
          "medium":  {
            "w": 600,
            "h": 600,
            "resize": "fit"
          },
          "large":  {
            "w": 720,
            "h": 720,
            "resize": "fit"
          }
        },
        "video_info":  {
          "aspect_ratio":  [
            1,
            1
          ],
          "duration_millis": 27886,
          "variants":  [
             {
              "content_type": "application/x-mpegURL",
              "url": "https://video.twimg.com/ext_tw_video/700760287205437440/pu/pl/AP9jZzzpsmucbs2J.m3u8"
            },
             {
              "bitrate": 1280000,
              "content_type": "video/mp4",
              "url": "https://video.twimg.com/ext_tw_video/700760287205437440/pu/vid/720x720/aQjrB6RYZqSHTmHh.mp4"
            },
             {
              "bitrate": 320000,
              "content_type": "video/mp4",
              "url": "https://video.twimg.com/ext_tw_video/700760287205437440/pu/vid/240x240/ct3QTyMNhoALuXoI.mp4"
            },
             {
              "bitrate": 832000,
              "content_type": "video/webm",
              "url": "https://video.twimg.com/ext_tw_video/700760287205437440/pu/vid/480x480/u5DsOczdH8Mgq4Bn.webm"
            },
             {
              "bitrate": 832000,
              "content_type": "video/mp4",
              "url": "https://video.twimg.com/ext_tw_video/700760287205437440/pu/vid/480x480/u5DsOczdH8Mgq4Bn.mp4"
            },
             {
              "content_type": "application/dash+xml",
              "url": "https://video.twimg.com/ext_tw_video/700760287205437440/pu/pl/AP9jZzzpsmucbs2J.mpd"
            }
          ]
        }
      }
    ]
  },
  "favorited": false,
  "retweeted": false,
  "possibly_sensitive": false,
  "possibly_sensitive_appealable": false,
  "lang": "en"
} ```
