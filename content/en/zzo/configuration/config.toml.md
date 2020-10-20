---
title: "config.toml"
date: 2020-10-18T17:01:32+09:00
draft: false
weight: 2
---

`config.toml` file is a Hugo itself configuration file. All the possible params are documented on [the official Hugo site](https://gohugo.io/getting-started/configuration/#all-configuration-settings).

### baseURL

Set this param to your site URL. Zzo theme is using this param for a search. So, if this param is not correct, the search won't work. If you bought a domain name, use it instead of a default one.

### theme

Theme to use (located by default in /themes/THEMENAME/).

### defaultContentLanguage 

Content without language indicator will default to this language.

### defaultContentLanguageInSubdir 

Render the default content language in subdir, e.g. `content/en/`. The site root `/` will then redirect to `/en/`.

### hasCJKLanguage

If true, auto-detect Chinese/Japanese/Korean Languages in the content. This will make `.Summary` and `.WordCount` behave correctly for CJK languages.

### summaryLength 

The length of text in words to show in a `.Summary`.

### buildFuture

Include content with publishdate in the future.

### copyright

Set your copyright text. You can use {year} to print current year. For example,
```
©{year} zzossig, All Rights Reserved
```
You can put link for [creativecommons](https://creativecommons.org/licenses/by-sa/4.0/)(or any links).
```
©2018 - {year} All content is licensed under <a target='_blank' rel='external noopener' href='https://example.com'>CC BY-SA</a>
```

### timeout

Timeout for generating page contents, in milliseconds (defaults to 10 seconds). Note: this is used to bail out of recursive content generation, if your pages are slow to generate (e.g., because they require large image processing or depend on remote contents) you might need to raise this limit.

### enableEmoji

Enable Emoji emoticons support for page content

### paginate

Default number of elements per page in [pagination](https://gohugo.io/templates/pagination/).

### rssLimit

Maximum number of items in the RSS feed.

### enableGitInfo

Enable .GitInfo object for each page (if the Hugo site is versioned by Git). This will then update the Lastmod parameter for each page using the last git commit date for that content file.

### googleAnalytics

Google Analytics tracking ID.

### markup

This is a markdown related configurations. See the [official documentation](https://gohugo.io/getting-started/configuration-markup).

### outputs

Used this param for the custom output `SearchIndex`. If you set `home = ["SearchIndex"]`, you can see the search index in the http(s)://www.mydomain.com/index.json.

### outputFormats

Used to define Custom output `SearchIndex`. It's a json file.

### taxonomies

Hugo includes support for user-defined groupings of content called taxonomies. Taxonomies are classifications of logical relationships between content.