---
title: "Config Files"
date: 2020-01-30T11:16:54+09:00
draft: false
weight: 1
enableToc: false
---

## Config folder structure

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

## config files

{{< expand "config.toml" >}}
```toml
baseURL = "http://example.org/" # The URL of your site.
title = "Hugo Zzo Theme" # Title of your site
theme = "zzo" # Name of Zzo theme folder in `themes/`.

defaultContentLanguage = "en" # Default language to use (if you setup multilingual)
defaultContentLanguageInSubdir = true # baseURL/en/, baseURL/kr/ ...
hasCJKLanguage = true # Set `true` for Chinese/Japanese/Korean languages.

summaryLength = 70 # The length of a post description on a list page.
buildFuture = true # if true, we can use future date for talks page

copyright = "©{year}, All Rights Reserved" # copyright symbol: $copy; current year: {year}
timeout = 10000
enableEmoji = true
paginate = 13 # Number of items per page in paginated lists.
rssLimit = 100

enableGitInfo = false # When true, the modified date will appear on a summary and single page. Since GitHub info needs to be fetched, this feature will slow down to build depending on a page number you have
googleAnalytics = ""

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
    endLevel = 3
    ordered = false
    startLevel = 2

[outputs]
  home = ["HTML", "RSS", "JSON"]

[taxonomies]
  category = "categories"
  tag = "tags"
  series = "series"
```
{{< /expand >}}

{{< expand "languages.toml" >}}
```toml
[en]
  title = "Hugo Zzo Theme"
  languageName = "English"
  weight = 1

[ko]
  title = "Hugo Zzo Theme"
  languageName = "한국어"
  weight = 2
```
{{< /expand >}}

{{< expand "menus.en.toml" >}}
```toml
[[main]]
  identifier = "about"
  name = "about"
  url = "about"
  weight = 1

[[main]]
  identifier = "archive"
  name = "archive"
  url = "archive"
  weight = 2

[[main]]
  identifier = "gallery"
  name = "gallery"
  url = "gallery"
  weight = 3
    
[[main]]
  parent = "gallery"
  name = "cartoon"
  url = "gallery/cartoon"

[[main]]
  parent = "gallery"
  name = "photo"
  url = "gallery/photo"

[[main]]
  identifier = "posts"
  name = "posts"
  url = "posts"
  weight = 4
    
[[main]]
  identifier = "notes"
  name = "notes"
  url = "notes"
  weight = 5
```
{{< /expand >}}

{{< expand "params.toml"  >}}
```toml
logoText = "Zzo" # Logo text that appears in the site navigation bar.
logoType = "short" # long, short -> short: squre shape includes logo text, long: rectangle shape not includes logo text
logo = true # Logo that appears in the site navigation bar.
description = "The Zzo theme for Hugo example site." # for SEO
custom_css = [] # custom_css = ["scss/custom.scss"] and then make file at root/assets/scss/custom.scss
custom_js = [] # custom_js = ["js/custom.js"] and then make file at root/assets/js/custom.js
useFaviconGenerator = false # https://www.favicon-generator.org/

themeOptions = ["dark", "light", "hacker", "solarized", "kimbie"] # select options for site color theme
notAllowedTypesInHome = ["contact", "talks", "about", "showcase"] # not allowed page types in home page. type can be set in front matter or default to folder name.
notAllowedTypesInHomeSidebar = ["about", "archive", "showcase"] # not allowed page types in home page sidebar(recent post titles).
notAllowedTypesInArchive = ["about", "talks", "showcase"] # not allowed page types in archive page

# header
homeHeaderType = "text" # text, img, slide

# navbar
enableThemeChange = true # site color theme

# body
enableBreadcrumb = true # breadcrumb for list, single page
enableSearch = true # site search with Fuse
enableSearchHighlight = true # when true, search keyword will be highlighted
enableGoToTop = true # scroll to top
enableWhoami = true # at the end of single page
summaryShape = "classic" # card, classic, compact
archiveGroupByDate = "2006" # "2006-01": group by month, "2006": group by year
archivePaginate = 13 # items per page
paginateWindow = 1 # setting it to 1 gives 7 buttons, 2 gives 9, etc. If set 1: [1 ... 4 5 6 ... 356] [1 2 3 4 5 ... 356] etc
talksPaginate = 8 # items per page
talksGroupByDate = "2006" # "2006-01": group by month, "2006": group by year

# whoami: usage - home page sidebar, single page bottom of post. all values can be empty
myname = "zzossig"
email = "zzossig@gmail.com"
whoami = "Web Developer"
bioImageUrl = "" # image url like http//... If not set, we find a avatar image in root/static/images/whoami/avatar.(png|jpg|svg)
useGravatar = false # we use this option highest priority
location = "Seoul, Korea"
organization = "Hugo"
link = "https://github.com/zzossig/hugo-theme-zzo"

# sidebar
enableBio = true # home page sidebar
enableSidebar = true # Set to false to create the full width of the content.
enableSidebarTags = true # if you want to use tags.
enableSidebarSeries = true
enableSidebarCategories = true
enableHomeSidebarTitles = true
enableListSidebarTitles = true
enableToc = true # single page table of contents, you can replace this param to toc(toc = true)
hideToc = false # Hide or Show toc
tocPosition = "inner" # inner, outer
enableTocSwitch = true # single page table of contents visibility switch
itemsPerCategory = 5 # maximum number of posts shown in the sidebar.
sidebarPosition = "right" # bio, profile component layout position

# footer
showPoweredBy = true # show footer text: Powered by Hugo and Zzo theme
showFeedLinks = true # RSS Feed 
showSocialLinks = true # email, facebook, twitter ...
enableLangChange = true # show button at bottom left of footer.

# service
baiduAnalytics = "" # alternative of google analytics
enableBusuanzi = false # if set true, total page view, total unique visitors show up in the footer.
busuanziSiteUV = true # unique visitors (total number of visitors)
busuanziSitePV = true # site total page view count
busuanziPagePV = true # post view count

# comment
enableComment = true
disqus_shortname = "" 
commento = false

[gitment]          # Gitment is a comment system based on GitHub issues. see https://github.com/imsun/gitment
  owner = ""              # Your GitHub ID
  repo = ""               # The repo to store comments
  clientId = ""           # Your client ID
  clientSecret = ""       # Your client secret

[utterances]       # https://utteranc.es/
  owner = ""              # Your GitHub ID
  repo = ""               # The repo to store comments

[gitalk]           # Gitalk is a comment system based on GitHub issues. see https://github.com/gitalk/gitalk
  owner = ""              # Your GitHub ID
  repo = ""               # The repo to store comments
  clientId = ""           # Your client ID
  clientSecret = ""       # Your client secret

# Valine.
# You can get your appid and appkey from https://leancloud.cn
# more info please open https://valine.js.org
[valine]
  enable = false
  appId = '你的appId'
  appKey = '你的appKey'
  notify = false  # mail notifier , https://github.com/xCss/Valine/wiki
  verify = false # Verification code
  avatar = 'mm' 
  placeholder = '说点什么吧...'
  visitor = false

[changyan]
  changyanAppid = ""        # Changyan app id             # 畅言
  changyanAppkey = ""       # Changyan app key

[livere]
  livereUID = ""            # LiveRe UID                  # 来必力

# Isso: https://posativ.org/isso/
[isso]
  enable = false
  scriptSrc = "" # "https://isso.example.com/js/embed.min.js"
  dataAttrs = "" # "data-isso='https://isso.example.com' data-isso-require-author='true'"

[socialOptions] # if set, social icons will show up.
  email = "mailto:your@email.com"
  phone = ""
  facebook = "http://example.org/"
  twitter = "http://example.org/"
  github = "https://github.com/zzossig/hugo-theme-zzo"
  stack-overflow = ""
  instagram = ""
  google-plus = ""
  youtube = ""
  medium = ""
  tumblr = ""
  linkedin = ""
  pinterest = ""
  stack-exchange = ""
  telegram = ""
  steam = ""
  weibo = ""
  douban = ""
  csdn = ""
  gitlab = ""
  mastodon = ""
  jianshu = ""
  zhihu = ""
  signal = ""
  whatsapp = ""

[donationOptions]
  enable = false # if set, the donation button will show up on the single page.
  alipay = "" # Alipay QR Code image (example path: images/donation/alipay-qrcode.png) and put your file at root/static/images/donation/
  wechat = "" # Wechat pay QR Code image (example path: same as above)
  paypal = "" # Paypal URL
  patreon = "" # Patreon URL
  bitcoin = "" # example path: images/donation/bitcoin-code-image.png

[copyrightOptions]
  enableCopyrightLink = false # if set, you can add copyright link
  copyrightLink = ""
  copyrightLinkImage = ""
  copyrightLinkText = ""

# possible share name: ["facebook","twitter", "reddit", "linkedin", "tumblr", "weibo", "douban", "line"]
[[share]]
  name = "facebook"
[[share]]
  name = "twitter"
  username = ""
```
{{</ expand >}}