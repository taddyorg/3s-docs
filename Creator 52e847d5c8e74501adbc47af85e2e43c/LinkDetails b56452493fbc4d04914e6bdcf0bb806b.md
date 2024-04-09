# LinkDetails

Describes how to generate an url to a creators’ website, email or social media accounts based on base_url, value, and type.

| Property | Type | Description |
| --- | --- | --- |
| type | LinkDetails%20b56452493fbc4d04914e6bdcf0bb806b.md | The website  |
| value | String | The specific path to append to the website to get to a creator’s profile |
| base_url | String (Optional, usually ignored) | Base url for the link. For security reasons this value is usually ignored by clients to avoid the following scenario: Setting a link type as TWITTER but linking to a malicious site that isn't http://twitter.com. Click https://gist.github.com/dmathewwws/f93499a77ee56ba5b4b8108716d58175 based on type. |

## LinkType

Possible website to use as a creators’ website, email or social media accounts

```jsx
enum LinkType {
  INSTAGRAM
  YOUTUBE
  TIKTOK
  PATREON
  KO_FI
  EMAIL
  TWITTER
  MASTODON
  FACEBOOK
  WEBSITE # can be any website that starts with https://
  MERCH_STORE # can be any website that starts with https://
  LINKTREE
  TWITCH
  SNAPCHAT
  REDDIT
  DISCORD
  TELEGRAM
  ETSY
  PINTEREST
  TUMBLR
  SPOTIFY
  SOUNDCLOUD
  BANDCAMP
  VIMEO
  WECHAT
  WHATSAPP
}
```

## Example

For the following links, let get the link to the creator’s twitter account:

We take the link with type = TWITTER, and append our [assumed base_url](https://gist.github.com/dmathewwws/f93499a77ee56ba5b4b8108716d58175) + value.

**Result:** [https://twitter.com/dmathewwws](https://twitter.com/dmathewwws)

```jsx
links": [
  {
    "type": "TWITTER",
    "base_url": "https://twitter.com/",
    "value": "dmathewwws"
  },
  {
    "type": "EMAIL",
    "value": "danny@taddy.org"
  },
  {
    "type": "WEBSITE",
    "base_url": "https://",
    "value": "bamcomics.art"
  }
],
```