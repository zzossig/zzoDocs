---
title: "Author"
date: 2020-01-30T11:54:22+09:00
draft: false
weight: 2
enableToc: false
---

## Multiple Author

Just set the author information in the front-matter.

```yaml
---
title:
...
author: # author name
authorEmoji: 🤖 # emoji for subtitle, summary meta data
authorImage: "/images/whoami/avatar.jpg" # image path in the static folder
authorImageUrl: "" # your image url. We use `authorImageUrl` first. If not set, we use `authorImage`.
authorDesc: # author description
socialOptions: # override params.toml file socialOptions
  email: ""
  facebook: ""
  ...
---
```
