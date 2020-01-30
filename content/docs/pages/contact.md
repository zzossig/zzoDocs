---
title: "Contact Page"
date: 2020-01-30T12:49:57+09:00
draft: false
weight: 2
enableToc: false
---

## formspree

Currently available service: **formspree**. Open an issue if you need another service vendor. 

1. Make a file at root/contact/index.md

```yaml
---
title: "Contact"
date: 2019-12-17T23:58:33+09:00
description: Contact page
type: contact
service: formspree
formId: "your@email.com"
---

This is contact page.
```

2. Add contact menu at root/config/_default/menus.en.toml.

```toml
...
[[main]]
  identifier = "contact"
  name = "contact"
  url = "contact"
  weight = 6
```

## default

If you want just a blank page and use a markdown, set the service param empty.
