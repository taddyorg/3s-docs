# ComicSeries

Display a comic series, including all comic issues and all images that make up the comic. (All properties are required unless stated otherwise)

| Property | Type | Description |
| --- | --- | --- |
| identifier | Uuid | Unique identifier for the comic |
| name | String | Name of the comic |
| description | String | A short description of the comic |
| status | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/SeriesStatus%20b25dcaa6c4ac49a99ccca37cec1ea07f.md | Status options for the comic |
| datePublished | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/Date%20df934cbbe3d643ec80ec68fe20edbcfe.md | Date the comic is published |
| url | String | Url link of this SSS feed |
| genres | [ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/Genre%205cbf121c556d46b3a3a1b75be120942c.md] | An array of what genres your comic. Most apps will only display use the first 2 or 3 genres provided. |
| tags | [String] | An array of tags for the comic.  Most apps will only display use the first 10 tags provided. |
| coverImage | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ImageDetails%20e20c0690a7124b8abba1e004e04415be.md | Cover art for the comic. Comes in 3 sizes (variants) cover_sm, cover_md, cover_lg |
| bannerImage | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ImageDetails%20e20c0690a7124b8abba1e004e04415be.md | Banner art for the comic. Comes in 3 sizes (variants) banner_sm, banner_md, banner_lg |
| thumbnailImage | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ImageDetails%20e20c0690a7124b8abba1e004e04415be.md | Thumbnail art for the comic. Comes in 1 size (variant) thumbnail |
| contentRating | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ContentRating%20a740d9ff98324542a1b7a6ec03e609ae.md | Rating for the comic. |
| inLanguage | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/Language%20a690b02a1d41497387f50c9076e49c84.md | Language the comic is in. |
| seriesType | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ComicSeriesType%206c51130eb3cd43c0be27de5cfc61d376.md | Type of comic |
| seriesLayout | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ComicSeriesLayout%209654104344a240d08820b8f144726dcc.md | Layout style for the comic |
| feedOwnerName | String | Name of the owner of this SSS feed. |
| feedOwnerEmail | String | Email used to verify ownership of this SSS feed. |
| copyrightNotice | String | Copyright details. |
| creators | [Creator%2052e847d5c8e74501adbc47af85e2e43c.md] | Links to Creator%2052e847d5c8e74501adbc47af85e2e43c.md. One for every creator for the comic. |
| issues | [ComicSeries%2050b66b484a3b40abad9f4c4311a6194c.md] | An array of all issues for the comic. |
| hostingProvider | Hosting%20Provider%206e7f341665344165a2e8aed178c47589.md | (Optional) Link to the Hosting%20Provider%206e7f341665344165a2e8aed178c47589.md. This gives you details on OAuth endpoints, which allow you to access paid content on this feed. |
| scopesForExclusiveContent | [String] | (Optional) If this comic series contain any exclusive content this property will be present. It lists the payment platforms which the user must use to view exclusive issues. |

## ComicIssue

Comic Series con contain multiple issues (episodes)

| Property | Type | Description |
| --- | --- | --- |
| identifier | Uuid | Unique identifier for the comic issue |
| name | String | Name of the issue |
| creatorNote | String | A note from the creator. Most apps will only display the first 260 characters. |
| datePublished | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/Date%20df934cbbe3d643ec80ec68fe20edbcfe.md | Date the issue is published. |
| bannerImage | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ImageDetails%20e20c0690a7124b8abba1e004e04415be.md | Banner art for the issue. Comes in 3 sizes (variants) banner_sm, banner_md, banner_lg |
| thumbnailImage | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ImageDetails%20e20c0690a7124b8abba1e004e04415be.md | Thumbnail art for the issue. Comes in 1 size (variant) thumbnail |
| stories | [ComicSeries%2050b66b484a3b40abad9f4c4311a6194c.md] | An array of all the stories (art) for the issue. |
| scopesForExclusiveContent | [String] | (Optional) This property will be present if this comic issue is exclusive content. It lists the payment platforms which the user must use to view exclusive issues. |
| dateExclusiveContentIsAvailable | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/Date%20df934cbbe3d643ec80ec68fe20edbcfe.md | (Optional) Date the exclusive issue is available for everyone. 

If this comic issue is exclusive content and will be free at a certain time in the future, this property will be present. This gives you the information to display ‘X days till Free’ for the comic issue.  |

## ComicStory

An image.

| Property | Type | Description |
| --- | --- | --- |
| identifier | Uuid | Unique identifier for the comic story (artwork) |
| storyImage | ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ImageDetails%20e20c0690a7124b8abba1e004e04415be.md | Art for the story. Comes in 1 size (variant) story |

### Example SSS Feed

[https://taddy.org/feeds/sss/comicseries/ffccf57d-0959-4eef-90dc-a8fe1c402deb](https://taddy.org/feeds/sss/comicseries/ffccf57d-0959-4eef-90dc-a8fe1c402deb)

### Comics Apps that support SSS Feeds

[Supported Comic Apps](ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/Supported%20Comic%20Apps%20c6d526905f2b45daaf724095a670d016.md)

### Want to notify comic apps about a new feed?

[https://taddy.org/developers/comics-api/add-a-comicseries-to-taddy](https://taddy.org/developers/comics-api/add-a-comicseries-to-taddy)

### Referenced types in this document:

[Language](ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/Language%20a690b02a1d41497387f50c9076e49c84.md)

[ImageDetails](ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ImageDetails%20e20c0690a7124b8abba1e004e04415be.md)

[ContentRating](ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ContentRating%20a740d9ff98324542a1b7a6ec03e609ae.md)

[ComicSeriesType](ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ComicSeriesType%206c51130eb3cd43c0be27de5cfc61d376.md)

[Genre](ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/Genre%205cbf121c556d46b3a3a1b75be120942c.md)

[Date](ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/Date%20df934cbbe3d643ec80ec68fe20edbcfe.md)

[SSSFeed](ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/SSSFeed%20b18c6f9cea98419a879d62c8aab622eb.md)

[SeriesStatus](ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/SeriesStatus%20b25dcaa6c4ac49a99ccca37cec1ea07f.md)

[ComicSeriesLayout](ComicSeries%2050b66b484a3b40abad9f4c4311a6194c/ComicSeriesLayout%209654104344a240d08820b8f144726dcc.md)

<aside>
❕ If you would like to edit or contribute to the SSS specification. You can either [submit a PR here](https://github.com/taddyorg/3s-docs) or by creating a notion account and [leaving a comment.](http://bit.ly/3VQqtQV)

Open Source Credit: This website is actually just a notion document. We use [Travis's notion + nextjs starter project](https://github.com/transitive-bullshit/nextjs-notion-starter-kit), you should check it out if you want an easy way to create + edit your docs.

</aside>