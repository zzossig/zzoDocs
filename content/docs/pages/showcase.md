---
title: "Showcase Page"
date: 2020-01-30T12:50:23+09:00
draft: false
weight: 4
enableToc: false
---

Showcase page is a listing page of project showcase. Follow the below steps to make it.

1. Make a file at `root/content/showcase/_index.md`.

    ```yaml
    ---
    title: "Showcase overview" # For SEO
    date: 2020-01-19T15:43:38+09:00
    description: My portfolio, repos, works overview page # For SEO
    enableBio: true # Set to false if you want to hide the bio component.
    ---
    ```

2. Make a category folder and a file at `root/content/showcase/hugo/_index.md`. (In my case, hugo is a category)

    ```yaml
    ---
    title: "Hugo" # category name
    date: 2020-01-19T21:04:11+09:00
    description: Hugo theme collection # For SEO
    category: theme # meta info appeared on a card bottom side. category in category
    categoryIcon: code # code, author, book, certificate, download, github, reviewer - default value is code
    enableBio: true
    ---
    ```

3. Make a file per project.

    `root/content/showcase/hugo/my-awesome-project.md`.

    ```yaml
    ---
    title: "My Awesome Project" # apperared on a card component
    date: 2020-01-19T21:13:42+09:00
    description: Hello world! This is my awesome project! # apperared on a card component
    weight: 1 # card ordering
    link: https://github.com/zzossig/hugo-theme-zzo
    repo: https://github.com/zzossig/hugo-theme-zzo
    pinned: true # appreared on a overview page.
    thumb: feature3/css3.png # relative path in static/images
    links:
    - name: # download
      icon: # download
      link: # https://github.com/gohugoio/hugo/releases/download/v0.64.1/hugo_extended_0.64.1_Windows-64bit.zip
    shields:
    - name: # GitHub stars
      image: # https://img.shields.io/github/stars/zzossig/hugo-theme-zdoc?label=Star&style=social
      link: # https://github.com/zzossig/hugo-theme-zdoc
    ---
    ```

4. Finally, make a menu at your root/config/_default/menus.en.toml file

    ```toml
    [[main]]
      identifier = "showcase"
      name = "Showcase"
      url = "showcase"
      weight = 7
    ```
