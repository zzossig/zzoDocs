---
title: "Archive Page"
date: 2020-01-30T12:50:46+09:00
draft: false
weight: -1
enableToc: false
---

Archive page is a page that list all of your post.

```yaml
---
title: Archive
date: 2020-01-30T12:50:46+09:00
type: archive
description: Zzo archive page
titleWrap: wrap # wrap, noWrap
---

```

You can exclude some sections that you don't want to display in the archive page.

In your `params.toml` file,

```toml
...
notAllowedTypesInArchive = ["about", "talks", "showcase", "gallery"]
...
```
