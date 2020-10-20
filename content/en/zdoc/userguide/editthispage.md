---
title: "Edit This Page"
date: 2020-10-21T06:39:22+09:00
draft: false
weight: 3
enableToc: false
---

The Edit-This-Page button is a page repository link.

1. If you want to show the button, set `enableEditBtn` to true in the `config.toml` file.

    ```config.toml
    ...
    enableEditBtn = true
    ...
    ```
2. Set the link base path. We have two options. You can set it globally or locally.

    - global: Set the `editBaseURL` param in the config.toml file.
        ```config.toml
        ...
        editBaseURL: "https://github.com/zzossig/zzoDocs/blob/master/content/en"
        ...
        ```
    - local: Set the `editBaseURL` param in the root section `_index.md` file. For example, we have two sections root in this site. `zzo` and `zdoc`. You can see the `Zzo theme` and `Zdoc theme` menu on the navigation bar. That is the root section.
        ```content/en/zdoc/_index.md {hl_lines=[5]}
        ---
        title: ""
        date: ""
        ...
        editBaseURL: "https://github.com/zzossig/zzoDocs/blob/master/content/en"
        ...
        ---
        ``` 