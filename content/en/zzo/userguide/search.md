---
title: "Search"
date: 2020-02-07T01:27:35+09:00
draft: false
weight: 7
enableToc: true
---

## prerequisite

Make sure you set the right `baseURL` in the `config.toml` file. Search working fine when you run your site locally even though you haven't set the `baseURL`. But it will make trouble when you deploy it to the server. See [the issue regarding this](https://github.com/zzossig/hugo-theme-zzo/issues/214).

## params.toml

There are few parameters related to the search.

```params.toml
enableSearch = true
enableSearchHighlight = true
enableAppbarSearchIcon = true
searchResultPosition = "main" # side, main
```

Check out the [params.toml document](/zzo/configuration/params.toml/#enablesearch) for mor information

## config.toml

Zzo theme make search index for the search. So, in order to use the search, you need to add this config params to `config.toml` file.

```config.toml
...
[outputs]
  home = ["HTML", "RSS", "SearchIndex"]
  section = ["HTML", "RSS", "SearchIndex"]
  taxonomyTerm = ["HTML", "RSS", "SearchIndex"]
  taxonomy = ["HTML", "RSS", "SearchIndex"]

[outputFormats]
  [outputFormats.SearchIndex]
    mediaType = "application/json"
    baseName = "index"
    isPlainText = true
    notAlternative = true
```

These config params make search index on home, section, taxonomy page.
