# Creator

Properties that make up a Creator SSS feed. (All properties are required unless stated otherwise)

| Property | Type | Description |
| --- | --- | --- |
| identifier | Uuid | Unique identifier for the creator |
| name | String | Name of the creator |
| bio | String | A short bio of the creator. Most apps will only display only the first 260 characters. |
| datePublished | Creator%2052e847d5c8e74501adbc47af85e2e43c/Date%20ea45186790894b0989f111f95a08b4db.md | Date the creator feed is published. |
| url | String | Url link of this SSS feed |
| tags | [String] | An array of tags for the creator.  Most apps will only display use the first 10 tags provided. |
| links | [Creator%2052e847d5c8e74501adbc47af85e2e43c/LinkDetails%20b56452493fbc4d04914e6bdcf0bb806b.md] | An array to links to a creator's website, email and social media accounts  |
| avatarImage | Creator%2052e847d5c8e74501adbc47af85e2e43c/ImageDetails%20562dc3abd57d4d56b737570fb30ea273.md | Avatar image for the creator. Comes in 3 sizes (variants) avatar_sm, avatar_md, avatar_lg |
| country | Creator%2052e847d5c8e74501adbc47af85e2e43c/Country%20297dae67f6cf46cabf31d8dfc3735c4b.md | Country the creator lives in or is from. |
| feedOwnerName | String | Name of the owner of this SSS feed. |
| feedOwnerEmail | String | Email use to verify ownership of this SSS feed. |
| copyrightNotice | String | Copyright details. |
| content | [Creator%2052e847d5c8e74501adbc47af85e2e43c.md] | An array of all the content by the creator and what roles they performed in making the content. |

## Content

Each issue (episode) that makes up a Comic Series

| Property | Type | Description |
| --- | --- | --- |
| @type | String | Type of the content (Must be a valid type from 3s-docs.org) |
| identifier | Uuid | Unique identifier for the content |
| url | String | Url link of the content’s SSS feed |
| roles | [Creator%2052e847d5c8e74501adbc47af85e2e43c/ContentRole%206360b121b5064b92b941b100ba1fb60e.md] | Roles performed by the creator in making this content. |

### Example SSS Feed

[https://taddy.org/feeds/sss/creator/8d3ed35e-4cf0-4986-bf20-4ee5bf4cfe05](https://taddy.org/feeds/sss/creator/8d3ed35e-4cf0-4986-bf20-4ee5bf4cfe05)

### Referenced types in this document:

[ContentRole](Creator%2052e847d5c8e74501adbc47af85e2e43c/ContentRole%206360b121b5064b92b941b100ba1fb60e.md)

[ImageDetails](Creator%2052e847d5c8e74501adbc47af85e2e43c/ImageDetails%20562dc3abd57d4d56b737570fb30ea273.md)

[LinkDetails](Creator%2052e847d5c8e74501adbc47af85e2e43c/LinkDetails%20b56452493fbc4d04914e6bdcf0bb806b.md)

[Country](Creator%2052e847d5c8e74501adbc47af85e2e43c/Country%20297dae67f6cf46cabf31d8dfc3735c4b.md)

[Date](Creator%2052e847d5c8e74501adbc47af85e2e43c/Date%20ea45186790894b0989f111f95a08b4db.md)

<aside>
❕ If you would like to edit or contribute to the SSS specification. You can either [submit a PR here](https://github.com/taddyorg/3s-docs) or by creating a notion account and [leaving a comment.](http://bit.ly/3VQqtQV)

Open Source Credit: This website is actually just a notion document. We use [Travis's notion + nextjs starter project](https://github.com/transitive-bullshit/nextjs-notion-starter-kit), you should check it out if you want an easy way to create + edit your docs.

</aside>