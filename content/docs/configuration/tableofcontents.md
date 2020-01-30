---
title: "Table of Contents"
date: 2020-01-30T12:08:37+09:00
draft: false
weight: 5
enableToc: false
---

## config.toml

There are some `toc` related params in the `config.toml` file.

```toml
[markup.tableOfContents]
    endLevel = 3
    ordered = false
    startLevel = 2
```

You need to set this configuration parameter. Otherwise `toc` will malfunction. `startLevel` and` endLevel` means that you use at maximum `##` , and at minimum, `###` for the title of the post.

## params.toml

You can set the toc related params at `params.toml` file for the global.

- hideToc - Hide the toc in the first place. You can toggle the switch to show the toc later .
- enableToc - Toc disapear entirely in all posts.
- toc - Toc disapear entirely in all posts. This is Alias to `enableToc`
- enableTocContent - Toc in the main article, not in sidebar.
- tocPosition: When `inner`, toc will be inside the border. When `outer`, toc will be outside of the border

## front matter

You can set toc params for each post, by setting front matter. So basically, each post can have it's own toc params that override global config.

```yaml
---
title: myPost
date: 2020-01-30
hideToc:
enableToc:
enableTocContent:
tocPosition:
...
---
```
