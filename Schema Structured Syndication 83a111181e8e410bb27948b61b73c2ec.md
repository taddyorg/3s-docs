# Schema Structured Syndication

SSS (Schema Structured Syndication) is an open-source specification that makes it possible for creators to self-publish their content to any app that supports this specification. The benefit of self-publishing content is that a creator **retains all copyrights to their IP**, gets to **keep full creative control of their work**, and **aren’t tied to any one tech platform**. This website documents the format of what a SSS feed to make it easy for developers who want to build apps using SSS Feeds.

## Example

This is the [SSS feed](https://taddy.org/feeds/sss/comicseries/ffccf57d-0959-4eef-90dc-a8fe1c402deb) for the comic Infinite Colours. The feed conforms to the [ComicSeries](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/ComicSeries%2050b66b484a3b40abad9f4c4311a6194c.md) specification and contains all the properties needed to display a comic (eg: the comic's name, cover art, and all the episode art). The screenshot below shows how the [Inkverse](https://inkverse.co) app displays Infinite Colours - and any other comic that conforms to the [ComicSeries](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/ComicSeries%2050b66b484a3b40abad9f4c4311a6194c.md) specification.

![The SSS feed contains details of the comic’s name, cover art, and all the episode art.](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/sss-inkverse-explainer.png)

The SSS feed contains details of the comic’s name, cover art, and all the episode art.

## Is this a new idea?

No! This is exactly how podcasts work. RSS (Really Simple Syndication) is used as the open-source specification that powers all podcast apps.

![podcast-ecosystem.png](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/podcast-ecosystem.png)

Podcasting is very different to every other content platform (YouTube, Instagram, TikTok) because **no one tech company owns podcasts**. Creators can choose to self-host or choose a hosting tool while listeners can listen to podcasts on any podcast player (Apple, Spotify, Overcast, PocketCast etc). 

Another big difference in podcasting is that if a creator ever leaves a content platform like YouTube, Instagram, TikTok they lose the subscribers they have built up on the platform. This isn't the case in podcasts where every podcast is self-published by the creators. If the creator wants, they can switch hosting tools but keep the listeners on all podcast players. ie) creators own the distribution to the audience in podcasting.

## Why not just use RSS?

RSS is a very flexible specification that heavily inspires SSS. However, while SSS is very similar to RSS, we wanted to take the best parts of how RSS is used to power podcasts and fix some of the things that frustrated us.

**What we loved:** When creating an RSS [podcast feed](https://help.apple.com/itc/podcasts_connect/#/itcb54353390), you may notice the use of XML tags that aren’t part of the RSS specification like `<itunes:image>`, `<itunes:category>`, `<itunes:explicit>`, `<itunes:author>`, `<itunes:owner>`, `<itunes:type>`, `<itunes:episode>`, `<itunes:season>`, `<itunes:episodeType>`. These tags allow app developers to build a rich user experience tailored to consuming podcasts. We kept this idea with SSS. The SSS specification defines tags to build rich experiences for **a specific type of content** (comics, books, music, videos).  

**What frustrated us:** Working with XML, not having a schema to define how to share more types of content (not just podcasts), not having easy-to-access developer documentation to make it easy to build an app that is powered by feeds, and lastly RSS has no concept of paid content (it's a public document with links to other publicly accessible URLs) so there is no way to pay creators directly for premium content.

## What are some differences between SSS and RSS?

1. **SSS uses JSON, while RSS uses XML.**
2. **SSS uses schema.org vocabulary.** [schema.org](http://schema.org/) provides type definitions for various types of content, including comics, books, music, and video.
3. **[Premium content can be unlocked.](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/Hosting%20Provider%206e7f341665344165a2e8aed178c47589/OAuth%201fe171bbefaf46db880244635988ae5a.md)** SSS specifies how to allow certain content to be accessible only to Patreon backers or other paid users. An SSS feed is a public document, and therefore, all the links contained in the document are public. However, SSS also outlines how to label certain content as premium and create a valid token to access that content.
4. **Every SSS feed is required to have an ETag or Last-Modified header**. Every SSS feed must return either an etag or last-modified header in the response. This enables efficient checking to see if the content in the feed has changed, without having to download or examine its details.
5. **Every SSS feed is required to conform to [WebSub](https://www.w3.org/TR/websub/)**. Every SSS feed must publish its feed to a Websub Hub. This allows subscribers to the feed to be notified immediately when the feed has been updated (ie: new content is available).

## SSS feed types:

<aside>
🎨 [**ComicSeries](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/ComicSeries%2050b66b484a3b40abad9f4c4311a6194c.md) →** Display a comic series, including all comic issues and all images that make up the comic.

</aside>

<aside>
🧑‍🎨 **[Creator](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/Creator%2052e847d5c8e74501adbc47af85e2e43c.md) →** Details on the creator (name, avatar image, social media links).

</aside>

<aside>
🗄️ [Hosting Provider](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/Hosting%20Provider%206e7f341665344165a2e8aed178c47589.md) **→** Details on the hosting provider. OAuth endpoint details are listed, allowing you to access exclusive content on the SSS feeds.

</aside>

## License

SSS is an open-source specification offered under the terms of the [Creative Commons Attribution / Share Alike license](https://creativecommons.org/licenses/by-sa/4.0/).  

Links to Important Pages:

[ComicSeries](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/ComicSeries%2050b66b484a3b40abad9f4c4311a6194c.md)

[Creator](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/Creator%2052e847d5c8e74501adbc47af85e2e43c.md)

[Hosting Provider](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/Hosting%20Provider%206e7f341665344165a2e8aed178c47589.md)

[Supported Apps](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/Supported%20Apps%20abd87af85dbd45c09ba686d9c73288c6.md)

[Apps for content creators](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/Apps%20for%20content%20creators%209fbf00f49a884db19925836a94385b0e.md)

[Creator-Friendly Copyright Notice](Schema%20Structured%20Syndication%2083a111181e8e410bb27948b61b73c2ec/Creator-Friendly%20Copyright%20Notice%2069bdbb09b2804878b76ca7787026d917.md)

<aside>
❕ If you would like to edit or contribute to the SSS specification. You can either [submit a PR here](https://github.com/taddyorg/3s-docs) or by creating a notion account and [leaving a comment.](http://bit.ly/3VQqtQV)

Open Source Credit: This website is actually just a notion document. We use [Travis's notion + nextjs starter project](https://github.com/transitive-bullshit/nextjs-notion-starter-kit), you should check it out if you want an easy way to create + edit your docs.

</aside>