---
title: "Search"
date: 2020-02-07T01:27:35+09:00
draft: false
weight: 7
enableToc: false
---

1. Zzo theme make search index for the search. So, in order to use the search, you need to add this config params to `config.toml` file.

```toml
...
[outputs]
  page = ["HTML", "SearchIndex"]
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

These config params make search index on every page.

2. We have an option to the search results rendering position.

    your `params.toml` file,
    ```
    ...
    searchResultPosition = "main" # side, main
    ```