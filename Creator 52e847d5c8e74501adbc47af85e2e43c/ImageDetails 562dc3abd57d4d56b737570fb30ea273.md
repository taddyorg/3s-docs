# ImageDetails

Describes how to generate an image url, based on its base_url and the desired variant.

| Property | Type | Description |
| --- | --- | --- |
| base_url | String | Base url for the image |
| variant_name1 | String | The string to append to the base url to get the desired size / variant for the image |
| variant_name2 | String | The string to append to the base url to get the desired size / variant for the image |
| variant_name3 | String | The string to append to the base url to get the desired size / variant for the image |

## Example

For a Creator, avatarImage has 3 possible variants. `avatar_sm`, `avatar_md`, `avatar_lg`. 

To get the medium avatar image, take the provided image details, and append the base_url + the desired variant (avatar_md):

```jsx
"avatarImage": {
  "base_url": "https://ax1.taddy.org/87aa38ce-2960-4fde-83e6-e638a2d77b2d/04cc94b3-8eac-4a50-a06d-5d7ae5db3c05/",
  "avatar_sm": "avatar-sm.webp",
  "avatar_md": "avatar-md.webp",
  "avatar_lg": "avatar-lg.webp"
},
```

**Result:** [https://ax1.taddy.org/87aa38ce-2960-4fde-83e6-e638a2d77b2d/04cc94b3-8eac-4a50-a06d-5d7ae5db3c05/avatar-md.webp](https://ax1.taddy.org/87aa38ce-2960-4fde-83e6-e638a2d77b2d/04cc94b3-8eac-4a50-a06d-5d7ae5db3c05/avatar-md.webp)