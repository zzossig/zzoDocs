---
title: "Menu Depth"
date: 2020-10-21T06:24:22+09:00
draft: false
weight: 2
enableToc: false
---

## Deep Depth Folder Structure

```
userguide
├── Depth - 1
│   ├── _index.md
│   ├── Depth - 2
│   │   ├── _index.md
│   │   ├── Depth - 3
│   │   │   ├── _index.md
│   │   │   ├── menudepth.md
```
## How to make menu collapsible.

As you can see from the folder structure above, every root folders that are collapsible have an `_index.md` file. In that file, we define the menu to be collapsible. Set `collapsible` Front-Matter to true if you want a menu to be collapsible.

```_index.md {hl_lines=[7]}
---
title: "Depth - 3"
date: 2020-02-28T10:08:56+09:00
description: 
draft: false
weight: 1
collapsible: true
---
```

