---
title: "Multi Language"
date: 2020-01-30T15:34:13+09:00
draft: false
weight: 6
enableToc: false
---

To enable/disable the language translation button in the footer, edit the parameter `enableLangChange` in `params.toml`.

The default language of this theme is English. If you want to use another language, follow these steps

1. Make a menu file.

    ```
    root
    ├── config
    │   ├── _default
    │   │   ├── ...
    │   │   ├── menus.ko.toml
    ```

    ```toml
    [[main]]
      identifier = "about"
      name = "about"
      url = "/about/"
      weight = 1

    [[main]]
        identifier = "archive"
        name = "archive"
        url = "/archive/"
        weight = 2
    ...
    ```

    `config/_default/menus.ko.toml`

2. Make a content file. Add your language code before the md extension.

    ```
    hugo new about/index.ko.md
    hugo new posts/markdown-syntax.ko.md
    ...
    ```

3. Make an i18n file.

    ```toml
    [search-placeholder]
    other = "검색..."

    [summary-dateformat]
    other = "2006년 01월 02일"

    [tags]
    other = "태그"
    ...
    ```

    `i18n/ko.toml`

4. Edit config.toml file.

    ```toml
    defaultContentLanguage = "ko"
    defaultContentLanguageInSubdir = true
    hasCJKLanguage = true
    ```
