---
title: "Installation"
date: 2020-01-30T00:38:25+09:00
description: Installation description
draft: false
weight: 1
---

## Step 1: Install Hugo

This guide assumes that you already installed the [Hugo-extended](https://gohugo.io/getting-started/installing/) version.

## Step 2: Create a New Site

Create a new site by typing this. It will create some empty folders. I'm going to make a `mydocs` folder in this guide.

```
hugo new site mydocs
```

## Step 3: Add a Theme

You can download and unpack the theme manually from Github but it's easier to use git to clone the repo.

```
cd mydocs
git init
git clone https://github.com/zzossig/hugo-theme-zdoc.git themes/zdoc
```

If you use git to version control your site, highly recommended, it's best to add the zdoc theme as a submodule.
Go to your site root folder(`mydocs` folder in my case) and type the bellow.

```
cd mydocs
git init
git submodule add https://github.com/zzossig/hugo-theme-zzo.git themes/zdoc
```

## Step 4: Add Config Files

We have to make 4 config files to make the theme work. Check out the [config files](/zdoc/configuration/configfiles/) section.

- [config.toml] - We can set Hugo itself related configuration params.
- [languages.toml] - We can change language related settings.
- [menus.en.toml] - We can add or delete site menus.
- [params.toml] - The params in this file are used only in the zdoc theme.

If your blog is planning to support multiple languages, I recommend you to make a contry code folder first like [en], [ko], [fr] etc.
In this way, you can manage your contents more efficiently. And then you should specify contents folder in the `language.toml` file.

```:language.toml
[en]
  ...
  contentdir = "content/en"
  ...
```

Create your site menu by making `menus.en.toml` file. The `en` can be any contry code. I'm going to make a docs menu in this guide.

```:menus.en.toml
[[main]]
  identifier = "docs"
  name = "Docs"
  url = "docs"
  weight = 1
  ...
```

## Step 5: Add Some Content

I'm going to make `docs` folder in `root/content/en` folder. The menu's root folder should have `_index.md` file.

```:/content/en/docs/_index.md
---
title: "docs section"
date: 2019-03-26T08:47:11+01:00
description: All the list of my documentation
---
```

The params(title, date, description) above used for SEO(search engine optimization). We call the params as front-matter. Some front-matter used for SEO, others used for displaying contents, configuration, etc. Now, let's make a first markdown file. Make md file in the docs folder

```:/content/en/docs/myfirstdoc.md
---
title: "My First Document"
date: 2019-03-26T08:47:11+01:00
description: You will find some of the most common and helpful pages from our documentation.
draft: false
---

Your markdown here.
```


## Updating

From the root of your site:

```
git submodule update --remote --merge
```

## Run example site

From the root of themes/zdoc/exampleSite:

```
hugo server --themesDir ../..
```
