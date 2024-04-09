# ImageDetails

Describes how to generate an image url, based on its base_url and the desired variant.

| Property | Type | Description |
| --- | --- | --- |
| base_url | String | Base url for the image |
| variant_name1 | String | The string to append to the base url to get the desired size / variant for the image |
| variant_name2 | String | The string to append to the base url to get the desired size / variant for the image |
| variant_name3 | String | The string to append to the base url to get the desired size / variant for the image |

## Example

For a ComicSeries, coverImage has 3 possible variants. `cover_sm`, `cover_md`, `cover_lg`. 

To get the medium cover image, take the provided image details, and append the base_url + the desired variant (cover_md):

```jsx
"coverImage": {
  "base_url": "https://ax1.taddy.org/96cc49d7-a95d-4266-b408-b57c7d26a62e/83d75a4b-563d-4a8f-94cb-60b5c536665c/",
  "cover_sm": "cover-sm.webp",
  "cover_md": "cover-md.webp",
  "cover_lg": "cover-lg.webp"
},
```

**Result:** [https://ax1.taddy.org/96cc49d7-a95d-4266-b408-b57c7d26a62e/83d75a4b-563d-4a8f-94cb-60b5c536665c/cover-md.webp](https://ax1.taddy.org/96cc49d7-a95d-4266-b408-b57c7d26a62e/83d75a4b-563d-4a8f-94cb-60b5c536665c/cover-md.webp)