---
title: "Multi Language"
date: 2020-01-30T15:34:13+09:00
draft: false
weight: 6
enableToc: false
---

To enable/disable the multi language button in the footer, edit the parameter `enableLangChange` in `params.toml`. The default language of this theme is English. If you want to use another language, follow these steps

1. Make a menu file.

    ```
    root
    ├── config
    │   ├── _default
    │   │   ├── ...
    │   │   ├── menus.ko.toml
    ```

    ```menus.ko.toml
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

2.  Make a language-code folder. Then make a content file.

    ```
    root/content/ko/markdown-syntax.md
    root/content/ko/hugo-blog.md
    ...
    ```

    I made a `ko` folder in the `content` folder. In that way, we can easily organize our content by language.

3. Make an i18n file.

    ```ko.toml
    [search-placeholder]
    other = "검색..."

    [summary-dateformat]
    other = "2006년 01월 02일"

    [tags]
    other = "태그"
    ...
    ```

    We already have some i18n files. If there is your language among them, this process can be omitted.

    - en
    - eo
    - fa
    - fr
    - ko
    - zh

4. Edit config.toml file.

    ```toml
    defaultContentLanguage = "ko"
    defaultContentLanguageInSubdir = true
    hasCJKLanguage = true
    ```
