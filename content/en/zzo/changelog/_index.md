---
title: "Change Log"
date: 2020-01-30T10:10:56+09:00
draft: false
collapsible: false
weight: -1
---

### Dec 19, 2020 [(dcd0901)](https://github.com/zzossig/hugo-theme-zzo/commit/dcd0901)

Support CJK header link.
Now, you can use Chinese, Japanese or Korean folder, file name in the content folder.

### Dec 10, 2020 [(7c1c61b)](https://github.com/zzossig/hugo-theme-zzo/commit/7c1c61b)

Support Netlify Form - [How to add Netlify Form](/zzo/pages/contact/)

### Dec 9, 2020 [(621c83a)](https://github.com/zzossig/hugo-theme-zzo/commit/621c83a)

Table of Contents(toc) bug fix - long toc not showing properly

### Dec 1, 2020 [(13e290e)](https://github.com/zzossig/hugo-theme-zzo/commit/13e290e)

Support D3 library. - [How to use D3 library](/zzo/externallibrary/d3/)

### Nov 14, 2020 [(9a5a692)](https://github.com/zzossig/hugo-theme-zzo/commit/9a5a692)

Img shortcode bug fix - When you are using subdomains for your blog, img shortcode not worked properly.

### Nov 14, 2020 [(2e96cb4)](https://github.com/zzossig/hugo-theme-zzo/commit/2e96cb4)

Add option to change default emoji icon - Merged pull request from tabinurie/customicon
To set your custom emoji icons, edit the `params.toml` file.

```params.toml
...
writtenTimeIcon = "📅"
modifiedTimeIcon = "📝"
readingTimeIcon = "☕"
authorIcon = "✍️"
pagePvIcon = "👀"
tagIcon = "🏷️"
publicationIcon = "📚"
typeIcon = "🎯"
```

### Nov 14, 2020 [(d86ef73)](https://github.com/zzossig/hugo-theme-zzo/commit/d86ef73)

New share buttons - Merged from tabinurie/dev_share
delicious, feedly, google bookmark, hatena bookmark, pinterest, pocket

You can use it like this. In your `params.toml` file,

```params.toml
...
[[share]]
  name = "pinterest"
```

### Nov 5, 2020 [(d694f16)](https://github.com/zzossig/hugo-theme-zzo/commit/d694f16)

Now, you can use table, codeblock(with clipboard) markdown syntax in the about page.

### Oct 21, 2020 [(6ee166e)](https://github.com/zzossig/hugo-theme-zzo/commit/6ee166e)

Notice shortcode redesigned.
support subtitle shown next to the title.

```yaml
---
title: "my title"
subtitle: "my sub title"
---
contents
```

### Oct 16, 2020 [(11e7081)](https://github.com/zzossig/hugo-theme-zzo/commit/11e7081)

Gallery bug fixed - The error fixed when there is no `images` folder in the static folder.
you can add search, language icon in your appbar. Before this commit, you had to find those icons in the profile, footer section each.

```params.toml
...
enableAppbarSearchIcon = false
enableAppbarLangIcon = false
```

### July 24, 2020 [(6e4765e)](https://github.com/zzossig/hugo-theme-zzo/commit/6e4765e)

Now, you can use typewriter in your home header. - [How to use typewriter](/zzo/userguide/typewriteheader/)

### Jun 10, 2020 [(ceef390)](https://github.com/zzossig/hugo-theme-zzo/commit/ceef390)

New param added - minItemsToShowInTagCloud
This option is useful when you have a bunch of tags that are only related to 1 article.

```params.toml
...
minItemsToShowInTagCloud = 1 # Minimum items to show in tag cloud
```