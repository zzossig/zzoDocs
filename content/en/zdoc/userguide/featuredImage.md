---
title: "Featured Image"
date: 2020-10-21T08:32:40+09:00
draft: false
weight: 5
enableToc: false
image: "images/mountain.jpg"
---

The featured-Image shortcode displays an image you set in the `image` Front-Matter. Note that when the `image` front-matter is set, the image appears in a post summary list.

{{< featuredImage alt="featured image" >}}

## How to use

You can use the `{{</* featuredImage */>}}` shortcode anywhere in your post. The image path is relative to the static folder. So, in the below case, the image is in the `root/static/images/mountain.jpg`.

```yaml {hl_lines=[4, 8]}
---
title: ""
...
image: "images/mountain.jpg"
...
---

{{</* featuredImage */>}}
...
```

You can also set optional params like this. `{{</* featuredImage alt="featured image" width=50 height=50 */>}}`

```yaml {hl_lines=[4, 7]}
---
title:
...
image: images/my-featured-image.png
---

{{</* featuredImage alt="featured image" width=50 height=50 */>}}
...
```
