---
title: "params.toml"
date: 2020-10-19T05:12:05+09:00
draft: false
weight: 5
---

The parameters in this file is used only in the zzo theme.

### logoText

Logo text appears in the navigation bar.

```>:params.toml
logoText = "Zzo"
```

{{< expand "logoText" >}}
  ![Zzo theme param - logoText](/images/configuration/zzo/params.toml/1.logoText.png)
{{< /expand >}}

### logoType

- short: default. Treat the logo as a square.
- long: Treat the logo as a rectangle.

```>:params.toml
logoType = "short"
```

{{< expand "logoType" >}}
  ![Zzo theme param - logoType](/images/configuration/zzo/params.toml/2.logoType.png)
{{< /expand >}}

### description

Used for Search Engine Optimization(SEO)

```>:params.toml
description = "My Awesome Blog!"
```

{{< expand "description" >}}
  ![Zzo theme param - description](/images/configuration/zzo/params.toml/3.description.png)
{{< /expand >}}

### useFaviconGenerator

Whether you want to use [favicon-generator](https://www.favicon-generator.org/) or not. See the [favicon user guide](/zzo/userguide/favicon) if you want to set this param to true.

```>:params.toml
useFaviconGenerator = true
```

{{< expand "useFaviconGenerator" >}}
  ![Zzo theme param - useFaviconGenerator](/images/configuration/zzo/params.toml/4.useFaviconGenerator.png)
{{< /expand >}}

### meta_image

When you want to share your blog posts to social media(Twitter, Facebook, Telegram, etc), your posts link can serve meta image as a link preview. See the [meta image user guide](/zzo/userguide/metaimage).

The meta_image param uses a relative path for a static folder. So, if your meta image exists in `root/static/images/meta/mymetaimage.jpg`, meta_image value should be `/images/meta/mymetaimage.jpg`

```>:params.toml
meta_image = "/images/meta/mymetaimage.jpg"
```

{{< expand "meta_image" >}}
  ![Zzo theme param - meta_image](/images/configuration/zzo/params.toml/5.meta_image.jpg)
{{< /expand >}}

### themeOptions

Color schemes that are used in this theme. We have 5 options. Delete some options if you don't want to include in your blog.

- hacker
- light
- dark
- solarized
- kimbie

```>:params.toml
themeOptions = ["light", "dark"]
```

{{< expand "themeOptions" >}}
  ![Zzo theme param - themeOptions](/images/configuration/zzo/params.toml/6.themeOptions.png)
{{< /expand >}}

### notAllowedTypesInHome

For example, you probably don't want to include `contact` page in your post list on the home page. Add some types that you don't want to include. There are many types used in this theme.

- about
- archive
- contact
- talks
- showcase
- publication
- presentation
- resume
- gallery


```>:params.toml
notAllowedTypesInHome = ["contact", "talks", "about", "showcase", "publication", "presentation", "resume"]
```

{{< expand "notAllowedTypesInHome" >}}
  ![Zzo theme param - notAllowedTypesInHome](/images/configuration/zzo/params.toml/7.notAllowedTypesInHome.png)
{{< /expand >}}

### notAllowedTypesInHomeSidebar

Types that you don't want to include on your home sidebar. See the [type list](/zzo/configuration/zzo/params.toml/#notallowedtypesinhome) here.

```>:params.toml
notAllowedTypesInHomeSidebar = ["about", "archive", "showcase", "gallery", "publication", "presentation", "resume"]
```

{{< expand "notAllowedTypesInHomeSidebar" >}}
  ![Zzo theme param - notAllowedTypesInHomeSidebar](/images/configuration/zzo/params.toml/8.notAllowedTypesInHomeSidebar.png)
{{< /expand >}}

### notAllowedTypesInArchive

Types that you don't want to include on your archive page. See the [type list](/zzo/configuration/zzo/params.toml/#notallowedtypesinhome) here.

```>:params.toml
notAllowedTypesInArchive = ["about", "talks", "showcase", "publication", "presentation", "resume"]
```

{{< expand "notAllowedTypesInArchive" >}}
  ![Zzo theme param - notAllowedTypesInArchive](/images/configuration/zzo/params.toml/9.notAllowedTypesInArchive.png)
{{< /expand >}}

### notAllowedTypesInHomeFeed

Types that you don't want to include on your RSS feed page. See the [type list](/zzo/configuration/zzo/params.toml/#notallowedtypesinhome) here.

```>:params.toml
notAllowedTypesInHomeFeed = ["about", "archive", "contact", "talks", "showcase", "publication", "presentation", "resume", "gallery"]
```

{{< expand "notAllowedTypesInHomeFeed" >}}
  ![Zzo theme param - notAllowedTypesInHomeFeed](/images/configuration/zzo/params.toml/10.notAllowedTypesInHomeFeed.png)
{{< /expand >}}

### viewportSize

You can expand or narrow your blog page as a whole. There are 5 options.

- widest
- wider
- wide
- normal
- narrow

```>:params.toml
viewportSize = "normal"
```

{{< expand "viewportSize" >}}
  ![Zzo theme param - viewportSize](/images/configuration/zzo/params.toml/11.viewportSize-narrow.png)
  ![Zzo theme param - viewportSize](/images/configuration/zzo/params.toml/11.viewportSize-widest.png)
{{< /expand >}}

### enableUiAnimation

Option for enabling or disabling UI animation when contents loaded.

```>:params.toml
enableUiAnimation = true
```

{{< expand "enableUiAnimation" >}}
  ![Zzo theme param - enableUiAnimation](/images/configuration/zzo/params.toml/12.enableUiAnimation.gif)
{{< /expand >}}

### hideSingleContentsWhenJSDisabled

If true, blog contents will be hidden when javascript disabled in a browser.

```>:params.toml
hideSingleContentsWhenJSDisabled = false
```

{{< expand "hideSingleContentsWhenJSDisabled" >}}
  ![Zzo theme param - hideSingleContentsWhenJSDisabled](/images/configuration/zzo/params.toml/13.hideSingleContentsWhenJSDisabled.png)
{{< /expand >}}

### minItemsToShowInTagCloud

Option to hide a small number of tags(series, categories)

```>:params.toml
minItemsToShowInTagCloud = 1
```

{{< expand "minItemsToShowInTagCloud" >}}
  ![Zzo theme param - minItemsToShowInTagCloud](/images/configuration/zzo/params.toml/14.minItemsToShowInTagCloud.png)
{{< /expand >}}

### enablePinnedPosts

When true, you can set `pinned` front-matter in a post. Pinned post appears on top of your post list.

```>:params.toml
enablePinnedPosts = true
```

{{< expand "enablePinnedPosts" >}}
  ![Zzo theme param - enablePinnedPosts](/images/configuration/zzo/params.toml/15.enablePinnedPosts.png)
{{< /expand >}}

### enableAppbarSearchIcon

When true, the search icon will appear in the navigation bar

```>:params.toml
enableAppbarSearchIcon = true
```

{{< expand "enableAppbarSearchIcon" >}}
  ![Zzo theme param - enableAppbarSearchIcon](/images/configuration/zzo/params.toml/16.enableAppbarSearchIcon.png)
{{< /expand >}}

### enableAppbarLangIcon

When true, the language icon will appear in the navigation bar

```>:params.toml
enableAppbarLangIcon = true
```

{{< expand "enableAppbarLangIcon" >}}
  ![Zzo theme param - enableAppbarLangIcon](/images/configuration/zzo/params.toml/17.enableAppbarLangIcon.png)
{{< /expand >}}

### homeHeaderType

```>:params.toml
homeHeaderType = "text"
```

{{< expand "homeHeaderType" >}}
  ![Zzo theme param - homeHeaderType](/images/configuration/zzo/params.toml/18.homeHeaderType.png)
{{< /expand >}}

### hideHomeHeaderWhenMobile

Hide home header when on mobile.

```>:params.toml
hideHomeHeaderWhenMobile = false
```

{{< expand "hideHomeHeaderWhenMobile" >}}
  ![Zzo theme param - hideHomeHeaderWhenMobile](/images/configuration/zzo/params.toml/19.hideHomeHeaderWhenMobile.png)
{{< /expand >}}

### showMobileMenuTerms

When true, you can have a [taxonomies](https://gohugo.io/content-management/taxonomies) menu on mobile.

```>:params.toml
showMobileMenuTerms = ["tags", "categories", "series"]
```

{{< expand "showMobileMenuTerms" >}}
  ![Zzo theme param - showMobileMenuTerms](/images/configuration/zzo/params.toml/20.showMobileMenuTerms.png)
{{< /expand >}}

### enableBreadcrumb

```>:params.toml
enableBreadcrumb = true
```

{{< expand "enableBreadcrumb" >}}
  ![Zzo theme param - enableBreadcrumb](/images/configuration/zzo/params.toml/21.enableBreadcrumb.png)
{{< /expand >}}

### enableSearch

Set to true if you want to enable the search feature.

```>:params.toml
enableSearch = true
```

{{< expand "enableSearch" >}}
  ![Zzo theme param - enableSearch](/images/configuration/zzo/params.toml/22.enableSearch.png)
{{< /expand >}}

### enableSearchHighlight

When true, search text will be colorized.

```>:params.toml
enableSearchHighlight = true
```

{{< expand "enableSearchHighlight" >}}
  ![Zzo theme param - enableSearchHighlight](/images/configuration/zzo/params.toml/23.enableSearchHighlight.png)
{{< /expand >}}

### enableGoToTop

```>:params.toml
enableGoToTop = true
```

{{< expand "enableGoToTop" >}}
  ![Zzo theme param - enableGoToTop](/images/configuration/zzo/params.toml/24.enableGoToTop.png)
{{< /expand >}}

### enableWhoami

```>:params.toml
enableWhoami = true
```

{{< expand "enableWhoami" >}}
  ![Zzo theme param - enableWhoami](/images/configuration/zzo/params.toml/25.enableWhoami.png)
{{< /expand >}}

### summaryShape

- card
- classic
- compact

```>:params.toml
summaryShape = "classic"
```

{{< expand "summaryShape" >}}
  ![Zzo theme param - summaryShape](/images/configuration/zzo/params.toml/26.summaryShape.png)
{{< /expand >}}

### searchResultPosition

- side
- main

```>:params.toml
searchResultPosition = "main"
```

{{< expand "searchResultPosition" >}}
  ![Zzo theme param - searchResultPosition](/images/configuration/zzo/params.toml/27.searchResultPosition.png)
{{< /expand >}}

### archiveGroupByDate

- "2006-01": group by month
- "2006": group by year

```>:params.toml
archiveGroupByDate = "2006"
```

{{< expand "archiveGroupByDate" >}}
  ![Zzo theme param - archiveGroupByDate](/images/configuration/zzo/params.toml/28.archiveGroupByDate.png)
{{< /expand >}}

### archivePaginate

A number of elements per page on the archive page.

```>:params.toml
archivePaginate = 20
```

{{< expand "archivePaginate" >}}
  ![Zzo theme param - archivePaginate](/images/configuration/zzo/params.toml/29.archivePaginate.png)
{{< /expand >}}

### paginateWindow

Setting it to 1 gives 7 buttons, 2 gives 9, etc. If set 1: [1 ... 4 5 6 ... 356] [1 2 3 4 5 ... 356] etc

```>:params.toml
paginateWindow = 1
```

{{< expand "paginateWindow" >}}
  ![Zzo theme param - paginateWindow](/images/configuration/zzo/params.toml/30.paginateWindow.png)
{{< /expand >}}

### talksPaginate

A number of elements per page on the talks page.

```>:params.toml
talksPaginate = 5
```

{{< expand "talksPaginate" >}}
  ![Zzo theme param - talksPaginate](/images/configuration/zzo/params.toml/31.talksPaginate.png)
{{< /expand >}}

### talksGroupByDate

- "2006-01": group by month
- "2006": group by year

```>:params.toml
talksGroupByDate = "2006"
```

{{< expand "talksGroupByDate" >}}
  ![Zzo theme param - talksGroupByDate](/images/configuration/zzo/params.toml/32.talksGroupByDate.png)
{{< /expand >}}

### pubPaginate

A number of elements per page on the publication page.

```>:params.toml
pubPaginate = 20
```

{{< expand "pubPaginate" >}}
  ![Zzo theme param - pubPaginate](/images/configuration/zzo/params.toml/33.pubPaginate.png)
{{< /expand >}}

### myname

Used for bio, whoami component

```>:params.toml
myname = "choi"
```

{{< expand "myname" >}}
  ![Zzo theme param - myname](/images/configuration/zzo/params.toml/34.myname.png)
{{< /expand >}}

### email

Used for bio, whoami component

```>:params.toml
email = "example@gmail.com"
```

{{< expand "email" >}}
  ![Zzo theme param - email](/images/configuration/zzo/params.toml/35.email.png)
{{< /expand >}}

### whoami

Used for bio, whoami component

```>:params.toml
whoami = "📚Learner🤓Nerd🌐Web Developer"
```

{{< expand "whoami" >}}
  ![Zzo theme param - whoami](/images/configuration/zzo/params.toml/36.whoami.png)
{{< /expand >}}

### bioImageUrl

Used for bio, whoami component. This param is for an external image link.

```>:params.toml
bioImageUrl = "https://..."
```

{{< expand "bioImageUrl" >}}
  ![Zzo theme param - bioImageUrl](/images/configuration/zzo/params.toml/37.bioImageUrl.png)
{{< /expand >}}

### useGravatar

Used for bio, whoami component. When true, the email param also needs to be correct.

```>:params.toml
useGravatar = false
```

{{< expand "useGravatar" >}}
  ![Zzo theme param - useGravatar](/images/configuration/zzo/params.toml/38.useGravatar.png)
{{< /expand >}}

### location

Used for bio, whoami component

```>:params.toml
location = "Seoul, Korea"
```

{{< expand "location" >}}
  ![Zzo theme param - location](/images/configuration/zzo/params.toml/39.location.png)
{{< /expand >}}

### organization

Used for bio, whoami component

```>:params.toml
organization = "Hugo"
```

{{< expand "organization" >}}
  ![Zzo theme param - organization](/images/configuration/zzo/params.toml/40.organization.png)
{{< /expand >}}

### link

Used for bio, whoami component

```>:params.toml
link = "https://zzossig.io"
```

{{< expand "link" >}}
  ![Zzo theme param - link](/images/configuration/zzo/params.toml/41.link.png)
{{< /expand >}}

### enableBio

```>:params.toml
enableBio = true
```

{{< expand "enableBio" >}}
  ![Zzo theme param - enableBio](/images/configuration/zzo/params.toml/42.enableBio.png)
{{< /expand >}}

### enableSidebar

```>:params.toml
enableSidebar = true
```

{{< expand "enableSidebar" >}}
  ![Zzo theme param - enableSidebar](/images/configuration/zzo/params.toml/43.enableSidebar.png)
{{< /expand >}}

### enableSidebarTags

```>:params.toml
enableSidebarTags = true
```

{{< expand "enableSidebarTags" >}}
  ![Zzo theme param - enableSidebarTags](/images/configuration/zzo/params.toml/44.enableSidebarTags.png)
{{< /expand >}}

### enableSidebarSeries

```>:params.toml
enableSidebarSeries = true
```

{{< expand "enableSidebarSeries" >}}
  ![Zzo theme param - enableSidebarSeries](/images/configuration/zzo/params.toml/45.enableSidebarSeries.png)
{{< /expand >}}

### enableSidebarCategories

```>:params.toml
enableSidebarCategories = true
```

{{< expand "enableSidebarCategories" >}}
  ![Zzo theme param - enableSidebarCategories](/images/configuration/zzo/params.toml/46.enableSidebarCategories.png)
{{< /expand >}}

### enableHomeSidebarTitles

```>:params.toml
enableHomeSidebarTitles = true
```

{{< expand "enableHomeSidebarTitles" >}}
  ![Zzo theme param - enableHomeSidebarTitles](/images/configuration/zzo/params.toml/47.enableHomeSidebarTitles.png)
{{< /expand >}}

### enableListSidebarTitles

```>:params.toml
enableListSidebarTitles = true
```

{{< expand "enableListSidebarTitles" >}}
  ![Zzo theme param - enableListSidebarTitles](/images/configuration/zzo/params.toml/48.enableListSidebarTitles.png)
{{< /expand >}}

### enableToc

Completely remove the table of contents(TOC).

```>:params.toml
enableToc = true
```

{{< expand "enableToc" >}}
  ![Zzo theme param - enableToc](/images/configuration/zzo/params.toml/49.enableToc.png)
{{< /expand >}}

### hideToc

Hide table of contents(TOC) temporary.

```>:params.toml
hideToc = false
```

{{< expand "hideToc" >}}
  ![Zzo theme param - hideToc](/images/configuration/zzo/params.toml/50.hideToc.png)
{{< /expand >}}

### tocFolding

When true, TOC will be folding dynamically.

```>:params.toml
tocFolding = true
```

{{< expand "tocFolding" >}}
  ![Zzo theme param - tocFolding](/images/configuration/zzo/params.toml/51.tocFolding.gif)
{{< /expand >}}

### tocPosition

- inner
- outer

```>:params.toml
tocPosition = "outer"
```

{{< expand "tocPosition" >}}
  ![Zzo theme param - tocPosition](/images/configuration/zzo/params.toml/52.tocPosition.png)
{{< /expand >}}

### enableTocSwitch

```>:params.toml
enableTocSwitch = true
```

{{< expand "enableTocSwitch" >}}
  ![Zzo theme param - enableTocSwitch](/images/configuration/zzo/params.toml/53.enableTocSwitch.png)
{{< /expand >}}

### itemsPerCategory

```>:params.toml
itemsPerCategory = 5
```

{{< expand "itemsPerCategory" >}}
  ![Zzo theme param - itemsPerCategory](/images/configuration/zzo/params.toml/54.itemsPerCategory.png)
{{< /expand >}}

### sidebarPosition

```>:params.toml
sidebarPosition = "right"
```

{{< expand "sidebarPosition" >}}
  ![Zzo theme param - sidebarPosition](/images/configuration/zzo/params.toml/55.sidebarPosition.png)
{{< /expand >}}

### showPoweredBy

```>:params.toml
showPoweredBy = true
```

{{< expand "showPoweredBy" >}}
  ![Zzo theme param - showPoweredBy](/images/configuration/zzo/params.toml/56.showPoweredBy.png)
{{< /expand >}}

### showFeedLinks

```>:params.toml
showFeedLinks = true
```

{{< expand "showFeedLinks" >}}
  ![Zzo theme param - showFeedLinks](/images/configuration/zzo/params.toml/57.showFeedLinks.png)
{{< /expand >}}

### showSocialLinks

```>:params.toml
showSocialLinks = true
```

{{< expand "showSocialLinks" >}}
  ![Zzo theme param - showSocialLinks](/images/configuration/zzo/params.toml/58.showSocialLinks.png)
{{< /expand >}}

### enableLangChange

```>:params.toml
enableLangChange = true
```

{{< expand "enableLangChange" >}}
  ![Zzo theme param - enableLangChange](/images/configuration/zzo/params.toml/59.enableLangChange.png)
{{< /expand >}}

### enableThemeChange

```>:params.toml
enableThemeChange = true
```

{{< expand "enableThemeChange" >}}
  ![Zzo theme param - enableThemeChange](/images/configuration/zzo/params.toml/60.enableThemeChange.png)
{{< /expand >}}

### googleTagManager

```>:params.toml
googleTagManager = "" # GTM-XXXXXX
```

### baiduAnalytics

```>:params.toml
baiduAnalytics = ""
```

### enableBusuanzi

```>:params.toml
enableBusuanzi = false
```

{{< expand "enableBusuanzi" >}}
  ![Zzo theme param - enableBusuanzi](/images/configuration/zzo/params.toml/61.enableBusuanzi.png)
{{< /expand >}}

### busuanziSiteUV

```>:params.toml
busuanziSiteUV = true
```

{{< expand "busuanziSiteUV" >}}
  ![Zzo theme param - busuanziSiteUV](/images/configuration/zzo/params.toml/62.busuanziSiteUV.png)
{{< /expand >}}

### busuanziSitePV

```>:params.toml
busuanziSitePV = true
```

{{< expand "busuanziSitePV" >}}
  ![Zzo theme param - busuanziSitePV](/images/configuration/zzo/params.toml/63.busuanziSitePV.png)
{{< /expand >}}

### busuanziPagePV

```>:params.toml
busuanziPagePV = true
```

{{< expand "busuanziPagePV" >}}
  ![Zzo theme param - busuanziPagePV](/images/configuration/zzo/params.toml/64.busuanziPagePV.png)
{{< /expand >}}

### updatePeriod

RSS update period

- hourly
- daily
- weekly
- monthly
- yearly

```>:params.toml
updatePeriod = "monthly"
```

### enableComment

Supported comment services

- disqus
- commento
- gitment
- utterances
- gitalk
- valine
- changyan
- livere
- isso

```>:params.toml
enableComment = false
```

{{< expand "enableComment" >}}
  ![Zzo theme param - enableComment](/images/configuration/zzo/params.toml/65.enableComment.png)
{{< /expand >}}

### socialOptions

If set, social icons will show up

- email
- phone
- facebook
- twitter
- github
- stack-overflow
- instagram
- google-plus
- youtube
- medium
- tumblr
- linkedin
- pinterest
- stack-exchange
- telegram
- steam
- weibo
- douban
- csdn
- gitlab
- mastodon
- jianshu
- zhihu
- signal
- whatsapp
- matrix
- xmpp
- dev-to
- gitea
- google-scholar
- twitch

```>:params.toml
[socialOptions]
  email = "mailto:your@email.com"
```

{{< expand "socialOptions" >}}
  ![Zzo theme param - socialOptions](/images/configuration/zzo/params.toml/66.socialOptions-bio.png)
  ![Zzo theme param - socialOptions](/images/configuration/zzo/params.toml/66.socialOptions-footer.png)
{{< /expand >}}

### donationOptions

- enable: If set, the donation button will appear at the end of the post.
- alipay: Alipay QR Code image (example path: images/donation/alipay-qrcode.png) and put your file at root/static/images/donation/
- wechat: Wechat pay QR Code image (example path: same as above)
- paypal: Paypal URL
- patreon: Patreon URL
- bitcoin: example path: images/donation/bitcoin-code-image.png

```>:params.toml
[donationOptions]
  enable = false
  alipay = ""
  wechat = ""
  bitcoin = ""
  paypal = ""
  patreon = ""
```

{{< expand "donationOptions" >}}
  ![Zzo theme param - donationOptions](/images/configuration/zzo/params.toml/67.donationOptions.png)
{{< /expand >}}

### share

If set, the social media button will appear at the end of the post.

- facebook
- twitter
- reddit
- linkedin
- tumblr
- weibo
- douban
- line
- whatsapp
- telegram

```>:params.toml
[[share]]
  name = "facebook"
[[share]]
  name = "twitter"
  username = ""
```

{{< expand "share" >}}
  ![Zzo theme param - share](/images/configuration/zzo/params.toml/68.share.png)
{{< /expand >}}