---
title: "Blog Page"
date: 2020-10-20T16:23:06+09:00
draft: false
weight: 2
enableToc: true
---

{{< expand "Blog Image" >}}
  ![Zdoc Blog Page](/images/pages/zdoc/zdoc-blog.png)
{{</ expand >}}

## Make blog step by step

1. Make a blog folder in your content root folder. In my case, it's `root/content/en/blog`
2. Make a `_index.md` file in the blog folder.
    ```root/content/en/blog/_index.md
    ---
    title: Blog
    description: My awesome blog
    ...
    ---
    ```
3. Add a blog menu to the navigation bar. You can add it in the `menus.en.toml` file.
    ```root/config/_default/menus.en.toml
    ...
    [[main]]
      identifier = "Blog"
      name = "Blog"
      url = "blog"
      weight = 3
    ```
4. Now, you can make some contents in the blog folder. Make a markdown file in this format. For the `tocLevels` Front-Matter, refer [this guide](https://zzo-docs.vercel.app/zzo/userguide/tableofcontents/#configtoml). There are no taxonomies other than tags.

    ```root/content/en/blog/myPost.md
    ---
    title: "My First Post"
    date: 2020-10-20T15:12:15+09:00
    draft: false
    weight: 1
    enableToc: true
    enableBlogBreadcrumb: false
    tocLevels: ["h2", "h3", "h4"]
    tags:
    - web
    - hugo
    ---
    ```

## Blog Header

There are two types of blog header. The images folder should be in the static folder. (/root/static/images/...)

- `text`
    ```root/content/en/blog/_index.md
    ---
    ...
    blogHeaderType: text
    header:
      - type: text
        height: 200
        paddingX: 50
        align: center
        title:
          - Blog
        subtitle: 
          - 
          - 
        titleColor: 
        titleFontSize: 44
        subtitleColor: 
        subtitleFontSize: 20
        spaceBetweenTitleSubtitle: 16
    ...
    ---
    ```
- `img`
    ```root/content/en/blog/_index.md
    ---
    ...
    blogHeaderType: img
    header:
      - type: img
        imageSrc: images/header/background.jpg
        imageSize: cover
        imageRepeat: no-repeat
        imagePosition: center
        height: 370
        paddingX: 50
        paddingY: 0
        align: center
        title:
          - Zzo blog
        subtitle:
          - 
        titleColor: 
        titleShadow: true
        titleFontSize: 44
        subtitleColor:
        subtitleFontSize: 16
        spaceBetweenTitleSubtitle: 20
    ...
    ---
    ```