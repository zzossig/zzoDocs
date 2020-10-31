---
title: "Table of Contents"
date: 2020-01-30T12:08:37+09:00
draft: false
weight: 5
enableToc: true
---

## Front-Matters

There are lots of TOC related params. You can not only set it in the `params.toml` file but also in the markdown file. If you set the TOC related params in `params.toml` file, it will be the global settings. If you set it in the front-matter, it will be the post-specific settings.

```yaml
---
title: "Table of Contents"
date: 2020-01-30T12:08:37+09:00
enableToc: true
hideToc: false
tocFolding: true
tocPosition: "outer"
enableTocSwitch: true
tocLevels = ["h2", "h3", "h4"]
---

```

Check out the toc related params [documentation](https://zzo-docs.vercel.app/zzo/configuration/params.toml/#enabletoc) to see what it is.

## config.toml

There are some `toc` related params in the `config.toml` file.

```toml
[markup.tableOfContents]
    endLevel = 3
    ordered = false
    startLevel = 2
```

You need to set this configuration parameter. Otherwise `toc` will malfunction. `startLevel` and` endLevel` means that you use at maximum `h2` tag , and at minimum, `h3` tag for the title of the post. And h1, h4, h5, h6 tags are not going to be included in your TOC element.

Some posts may have h2 tags and some posts may not. For that reason, I made `tocLevels` front-matter. So, it's best practice to use `todLevels` in every markdown file if you want to include TOC in your post.

```yaml
---
title:
date:
...
tocLevels: ["h2", "h3", "h4", "h5"]
---
```

## params.toml

You can set the toc related params at `params.toml` file for the global.

- hideToc - Hide the toc in the first place. You can toggle the switch to show the toc later .
- enableToc - Toc disapear entirely in all posts.
- toc - Toc disapear entirely in all posts. This is Alias to `enableToc`
- enableTocContent - Toc in the main article, not in sidebar.
- tocPosition: When `inner`, toc will be inside the border. When `outer`, toc will be outside of the border
