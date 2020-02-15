---
title: "Installation"
date: 2020-01-30T00:38:25+09:00
description: Installation description
draft: false
weight: 1
enableToc: false
---

You can download and unpack the theme manually from Github but it's easier to use git to clone the repo.

From the root of your site:

```
$ git clone https://github.com/zzossig/hugo-theme-zzo.git themes/zzo
```

If you use git to version control your site, highly recommended, it's best to add the zzo theme as a submodule.

From the root of your site:

```
git submodule add https://github.com/zzossig/hugo-theme-zzo.git themes/zzo
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
