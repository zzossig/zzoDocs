---
title: "Config Files"
date: 2020-01-30T11:16:54+09:00
draft: false
weight: 1
---

## Config Folder Structure

Keep in mind the underscore on the `_default` folder. You have to have all of these files, otherwise the theme doesn't work.

```
root
├── config
│   ├── _default
│   │   ├── config.toml
│   │   ├── languages.toml
│   │   ├── menus.en.toml
│   │   ├── params.toml
```

## Config Files

{{< expand "config.toml" >}}
```:/config/_default/config.toml
baseURL = "http://example.org/" # The URL of your site.
title = "Hugo Zzo Theme" # Title of your site
theme = "zzo" # Name of Zzo theme folder in `themes/`.

defaultContentLanguage = "en" # Default language to use (if you setup multilingual)
defaultContentLanguageInSubdir = true # baseURL/en/, baseURL/kr/ ...
hasCJKLanguage = true # Set `true` for Chinese/Japanese/Korean languages.

copyright = "©{year}, All Rights Reserved" # copyright symbol: $copy; current year: {year}
timeout = 10000
enableEmoji = true
paginate = 13 # Number of items per page in paginated lists.
rssLimit = 100

googleAnalytics = ""

disableKinds = ["taxonomyTerm"]

[markup]
  [markup.goldmark]
    [markup.goldmark.renderer]
      hardWraps = true
      unsafe = true
      xHTML = true
  [markup.highlight]
    codeFences = true
    lineNos = true
    lineNumbersInTable = true
    noClasses = false
  [markup.tableOfContents]
    endLevel = 4
    ordered = false
    startLevel = 2

[outputs]
  home = ["HTML", "RSS", "SearchIndex"]

[outputFormats]
  [outputFormats.SearchIndex]
    mediaType = "application/json"
    baseName = "index"
    isPlainText = true
    notAlternative = true
    
[taxonomies]
  tag = "tags"
```
{{< /expand >}}

{{< expand "languages.toml" >}}
```:/config/_default/languages.toml
[en]
  title = "Z Themes Documentation"
  languageName = "English"
  weight = 1
  languagedir = "ltr"
  contentdir = "content/en"
  
[ko]
  title = "Z Themes Documentation"
  languageName = "한국어"
  weight = 2
  languagedir = "ltr"
  contentdir = "content/en"
```
{{< /expand >}}

{{< expand "menus.en.toml" >}}
```:/config/_default/menus.en.toml
[[main]]
  identifier = "Zzo"
  name = "Zzo theme"
  url = "zzo"
  weight = 1

[[main]]
  identifier = "Zdoc"
  name = "Zdoc theme"
  url = "zdoc"
  weight = 2

[[main]]
  identifier = "Blog"
  name = "Blog"
  url = "blog"
  weight = 3
...
```
{{< /expand >}}

{{< expand "params.toml"  >}}
```:/config/_default/params.toml
logo = true
logoText = "Z Themes"
logoType = "short" # long, short
description = "The Zzo theme documentation site."
editBaseURL = "https://github.com/zzossig/zzoDocs/blob/master/content"
themeOptions = ["light", "dark"]

useFaviconGenerator = true # https://www.favicon-generator.org/

wideViewAsDefault = true

enableWideBlogSwitch = true
enableTocSwitch = true
enableLandingBackground = true
enableSearch = true
enableSearchHighlight = true
enableLangChange = true
enableDarkMode = true
enableBreadcrumb = true
enableBlogBreadcrumb = true
enableEditBtn = true
enableToc = true
enableMenu = true
enableNavbar = true
enableFooter = true
showPoweredBy = true

paginateWindow = 1
taxoPaginate = 13
taxoGroupByDate = "2006" # "2006-01": group by month, "2006": group by year

github = "https://github.com/zzossig/hugo-theme-zzo"

enableComment = false
[utterances]       # https://utteranc.es/
  owner = "zzossig"              # Your GitHub ID
  repo = "zzoDocs"               # The repo to store comments
{{</ expand >}}