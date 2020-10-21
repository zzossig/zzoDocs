---
title: "Footer Links"
date: 2020-10-21T06:39:22+09:00
draft: false
weight: 10
enableToc: false
---

You can add some links in your footer.

{{< img src="/images/userguide/zzo/footer-links.png" title="Zzo footer links" caption="Footer links look and feel" alt="Zzo footer links">}}

You just need to add some params in `params.toml` file. You can add as many as you want.

```params.toml
...
[[footerLinks]]
  name = "myLink1"
  link = "https://google.com"
[[footerLinks]]
  name = "myLink2"
  link = "https://yahoo.com"
```