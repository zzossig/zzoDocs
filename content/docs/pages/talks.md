---
title: "Talks Page"
date: 2020-01-30T12:49:51+09:00
draft: false
weight: 3
enableToc: false
---

Talks page is a listing page of links(video, ppt, event, ...). UI is similar to the archive page. Follow the below steps to make it.

1. Make a file at root/content/talks/_index.md.

    ```yaml
    ---
    title: "Talks"
    date: 2019-12-30T11:14:14+09:00
    description: Talks Page
    titleWrap: wrap # wrap, nowrap
    ---
    ```

2. Next, make some files under the `talks` folder you have created in step 1. If you want to make other link post, then make another file under the `talks` folder.

    root/content/talks/myLinks.md

    ```yaml
    ---
    title: "My Awesome links"
    date: 2019-12-31T00:04:50+09:00
    publishDate: 2019-12-31
    description:
    tags:
    -
    series:
    -
    categories:
    -
    ---
    ```

3. Finally, make a menu at your root/config/_default/menus.en.toml file

    ```toml
    [[main]]
      identifier = "talks"
      name = "talks"
      url = "talks"
      weight = 6
    ```

    And we are good to go.

4. Additionally, if you want to use a future date for the talks page, you need more things to do.

    - add config variable named `buildFuture` at root/config/_default/config.toml

    ```toml
    ...
    buildFuture = true
    ...
    ```

    - add publishDate front matter to your md file at root/content/talks/myLinks.md

    ```yaml
    ---
    title:
    date:
    publishDate: 2020-02-20
    ...
    ---
    ...
    ```