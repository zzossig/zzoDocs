---
title: "Presentation Page"
date: 2020-01-30T12:51:34+09:00
draft: false
weight: 5
enableToc: false
---

The presentation page uses `reveal.js`. I don't think anyone uses this page, including me. If you do think that this page is useful and want to get improved, or have some suggestions, open a new issue in [the zzo theme repository](https://github.com/zzossig/hugo-theme-zzo/issues).

## How to make presentation page

1. Make a file at `root/content/presentation/_index.md`.

    ```yaml
    ---
    title: "Presentations"
    description: "Presentation list with reveal.js"
    ---
    ```

2. And then, make a presentation markdown file. I made a `archetype` in the archetypes folder. You can take advantage of this file to make a markdown file by typing like this.

    ```
    hugo new --kind presentation presentation/mypt.md
    ```

    This line of code means that you want to make `mypt.md` file at `content/presentation` folder by using `presentation` archetype.