---
title: "Tab"
date: 2020-01-30T16:40:40+09:00
draft: false
weight: 8
enableToc: false
---

tab / tabs => Tabs make it easy to explore and switch between different views

`````
{{</* tabs Windows MacOS Ubuntu >}}
  {{</* tab */>}}

  ### Windows section

  ```javascript
  console.log('Hello World!');
  ```

  {{</* /tab */>}}
  {{</* tab */>}}

  ### MacOS section

  Hello world!
  {{</* /tab */>}}
  {{</* tab */>}}

  ### Ubuntu section

  Great!
  {{</* /tab */>}}
{{</* /tabs */>}}
`````

⚠️Becareful that the content in the tab should be different from each other.
The tab makes unique id hashes depending on the tab contents.
So, If you just copy-paste the tabs with multiple times, since it has the same contents, the tab will not work.

### image

{{< img src="/images/shortcodes/tab.png" title="Tab" caption="Zzo Tab shortcode" alt="image alt">}}