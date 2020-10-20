---
title: "featuredImage"
date: 2020-02-24T15:40:40+09:00
draft: false
weight: 9
enableToc: false
---

`featuredImage` shortcode displays the featured image specified in the `image` front-matter.

You can use `{{</* featuredImage */>}}` shortcode anywhere in your post.

You can also set optional params like this. `{{</* featuredImage alt="featured image" width=50 height=50 */>}}`

```yaml
---
title:
...
image: images/my-featured-image.png
---

{{</* featuredImage */>}}
```
