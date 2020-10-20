---
title: "Docs Page"
date: 2020-10-20T16:23:06+09:00
draft: false
weight: 3
enableToc: true
---

{{< expand "Document Page Image" >}}
  ![Zdoc Document Page](/images/pages/zdoc/zdoc-doc.png)
{{</ expand >}}

## Make document step by step

1. Add a document menu to the navigation bar. You can add it in the `menus.en.toml` file.
    ```root/config/_default/menus.en.toml
    ...
    [[main]]
      identifier = "docs"
      name = "Docs"
      url = "docs"
      weight = 1
    ```
2. Make a `docs` folder in your content root folder. The name `docs` is because I made the folder in step 1.
3. Make a `_index.md` file in the `docs` folder.
    ```root/content/en/docs/_index.md
    ---
    title: "Docs"
    description: "My first documentation"
    date: 2020-10-20T14:09:21+09:00
    draft: false
    ---
    ```
4. Now, you can make some markdown files in the docs folder.
    ```root/content/en/docs/installation.md
    ---
    title: "Installation"
    date: 2020-10-20T00:38:25+09:00
    description: Installation description
    draft: false
    weight: 1
    enableToc: true
    tocLevels: ["h2", "h3", "h4"]
    ---
    Your contents here.
    ```
5. But, you probably want to categorize your contents. Let's say, you want to make a `userguide` folder to categorize your contents. Make the folder first, and then make a `_index.md` file there.
    ```root/content/en/docs/userguide/_index.md
    ---
    title: "User Guide"
    date: 2020-01-30T10:10:56+09:00
    draft: false
    collapsible: true
    weight: 3
    ---
    ...
    ```
    There is a `collapsible` Front-Matter. When it is true, that markdown file becomes a collapsible menu. Now, you can make some markdown files in the userguide folder like this.
    ```root/content/en/docs/userguide/search.md
    ---
    title: "Search"
    description: "This is a search documentation"
    date: 2020-10-20T01:27:35+09:00
    draft: false
    weight: 7
    enableToc: true
    tocLevels: ["h2", "h3", "h4"]
    ---
    ...
    ```