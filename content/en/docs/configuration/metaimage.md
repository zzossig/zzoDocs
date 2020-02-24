---
title: "Meta Image"
date: 2020-02-01T18:49:15+09:00
draft: false
weight: 0
enableToc: false
---

We have front matter for the images used in link preview(twitter, facebook, etc...)
If the meta_image front-matter is not set, `image` front-matter will be used instead(as a default value).

```yaml
---
title:
date:
...
meta_image: images/posts/myMetaImage.png
---
```

The `meta_image` path is relative to the static folder. In the above example, image should be in the `root/static/images/posts` folder.

{{< img src="/images/configuration/linkpreview.png" title="Link Preview" caption="twitter card" alt="twitter card">}}