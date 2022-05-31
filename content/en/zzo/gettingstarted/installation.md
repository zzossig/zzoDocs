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

Create a new site by typing this. It will create some empty folders. I'm going to make a `myblog` folder in this guide.

```
hugo new site myblog
```

## Step 3: Add a Theme

You can download and unpack the theme manually from Github but it's easier to use git to clone the repo.

```
cd myblog
git init
git clone https://github.com/zzossig/hugo-theme-zzo.git themes/zzo
```

If you use git to version control your site, highly recommended, it's best to add the zzo theme as a submodule.
Go to your blog root folder(`myblog` folder in my case) and type the bellow.

```
cd myblog
git init
git submodule add https://github.com/zzossig/hugo-theme-zzo.git themes/zzo
```

## Step 4: Add Config Files

We have to make 4 config files to make the theme work. Check out the [config files](/zzo/configuration/configfiles/) section.

- [config.toml] - We can set Hugo itself related configuration params.
- [languages.toml] - We can change language related settings.
- [menus.en.toml] - We can add or delete site menus.
- [params.toml] - The params in this file are used only in the zzo theme.

If your blog is planning to support multiple languages, I recommend you to make a country code folder first like [en], [ko], [fr] etc.
In this way, you can manage your contents more efficiently. And then you should specify contents folder in the `language.toml` file.

```:language.toml
[en]
  ...
  contentdir = "content/en"
  ...
```

Create your blog menu by making `menus.en.toml` file. The `en` can be any country code. I'm going to make a posts menu in this guide.

```:menus.en.toml
[[main]]
  identifier = "posts"
  name = "Posts"
  url = "posts"
  weight = 1
  ...
```

## Step 5: Add Some Content

I'm going to make `posts` folder in `root/content/en` folder. The menu's root folder should have `_index.md` file.

```:/content/en/posts/_index.md
---
title: "Post section"
date: 2019-03-26T08:47:11+01:00
description: All the list of my posts
---
```

The params(title, date, description) above used for SEO(search engine optimization). We call the params as front-matter. Some front-matter used for SEO, others used for displaying contents, configuration, etc. Now, let's make a first post. Make md file in the posts folder

```:/content/en/posts/myfirstpost.md
---
title: "My First Post"
date: 2019-03-26T08:47:11+01:00
description: This is my awesome post!
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

From the root of themes/zzo/exampleSite:

```
hugo server --themesDir ../..
```
