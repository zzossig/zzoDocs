---
title: "Copyright"
date: 2020-01-30T15:40:24+09:00
draft: false
weight: 4
enableToc: false
---

If you want to add a link to the footer copyright, not just a text, you can customize it.

1. In your config.toml file, set the copyright param like this.

    ```toml
    ...
    copyright = This is my {} copyright text
    ...
    ```

    The {} part will be your copyright link.

    You can use markdown syntax for a link.

    ```toml
    ...
    copyright = [zzossig](https://zzossig.io) - All right reserved
    ...
    ```

2. In your params.toml file, set the copyrightOptions params

    ```toml
    ...
    [copyrightOptions]
      enableCopyrightLink = false
      copyrightLink = "https://..."
      copyrightLinkImage = "https://..."
      copyrightLinkText = "copyright link text"
    ```

3. For example, I set this params like this.

    ```toml
    ...
    [copyrightOptions]
      enableCopyrightLink = true
      copyrightLink = "http://creativecommons.org/licenses/by-sa/4.0/"
      copyrightLinkImage = ""
      copyrightLinkText = "CC BY-SA"
    ```