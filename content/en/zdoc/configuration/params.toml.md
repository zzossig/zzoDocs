---
title: "params.toml"
date: 2020-10-19T05:12:05+09:00
draft: false
weight: 5
---

The parameters in this file is used only in the zdoc theme.

### logo

Whether you want to use a logo icon in the navigation bar or not.

```>:params.toml
logo = true
```

{{< expand "logo" >}}
  ![Zdoc theme param - logoText](/images/configuration/zdoc/params.toml/1.logo.png)
{{< /expand >}}

### logoText

Logo text appears in the navigation bar.

```>:params.toml
logoText = "Z Themes"
```

{{< expand "logoText" >}}
  ![Zdoc theme param - logoText](/images/configuration/zdoc/params.toml/2.logoText.png)
{{< /expand >}}

### logoType

- short: default. Treat the logo as a square.
- long: Treat the logo as a rectangle.

```>:params.toml
logoType = "short"
```

{{< expand "logoType" >}}
  ![Zdoc theme param - logoType](/images/configuration/zdoc/params.toml/1.logo.png)
{{< /expand >}}

### description

Used for Search Engine Optimization(SEO)

```>:params.toml
description = "My Awesome Blog!"
```

### useFaviconGenerator

Whether you want to use [favicon-generator](https://www.favicon-generator.org/) or not. See the [favicon user guide](/zzo/userguide/favicon) if you want to set this param to true.

```>:params.toml
useFaviconGenerator = true
```

{{< expand "useFaviconGenerator" >}}
  ![Zdoc theme param - useFaviconGenerator](/images/configuration/zdoc/params.toml/3.favicon.png)
{{< /expand >}}

### wideViewAsDefault

Set it true when you want a wide page view. If true, TOC or menu sidebar will be folded as default.

```>:params.toml
wideViewAsDefault = true
```

{{< expand "wideViewAsDefault" >}}
  - `true`
    ![Zdoc theme param - wideViewAsDefault](/images/configuration/zdoc/params.toml/4.wideview-1.png)
  - `false` 
    ![Zdoc theme param - wideViewAsDefault](/images/configuration/zdoc/params.toml/4.wideview-2.png)
{{< /expand >}}

### enableWideBlogSwitch

When true, a viewport-sizing toggle button will appear on a blog post page.

```>:params.toml
enableWideBlogSwitch = true
```

{{< expand "enableWideBlogSwitch" >}}
  ![Zdoc theme param - enableWideBlogSwitch](/images/configuration/zdoc/params.toml/5.wideblogswitch.png)
{{< /expand >}}

### enableTocSwitch

When true, a toc-visibility toggle button will appear on a blog post page.

```>:params.toml
enableTocSwitch = true
```

{{< expand "enableTocSwitch" >}}
  ![Zdoc theme param - enableTocSwitch](/images/configuration/zdoc/params.toml/6.tocswitch.png)
{{< /expand >}}

### enableSearch

Set to true if you want to enable the search feature.

```>:params.toml
enableSearch = true
```

{{< expand "enableSearch" >}}
  ![Zdoc theme param - enableSearch](/images/configuration/zdoc/params.toml/7.enableSearch.png)
{{< /expand >}}

### enableSearchHighlight

When true, search text will be colorized.

```>:params.toml
enableSearchHighlight = true
```

{{< expand "enableSearchHighlight" >}}
  ![Zdoc theme param - enableSearchHighlight](/images/configuration/zdoc/params.toml/8.enableSearchHighlight.png)
{{< /expand >}}

### enableLangChange

```>:params.toml
enableLangChange = true
```

{{< expand "enableLangChange" >}}
  ![Zdoc theme param - enableLangChange](/images/configuration/zdoc/params.toml/9.enableLangChange.png)
{{< /expand >}}

### enableDarkMode

When true, a theming toggle button will appear on the navigation bar.

```>:params.toml
enableDarkMode = true
```

{{< expand "enableDarkMode" >}}
  ![Zdoc theme param - enableDarkMode](/images/configuration/zdoc/params.toml/10.enableDarkMode.png)
{{< /expand >}}

### enableBreadcrumb

When false, breadcrumb will disappear on every document page.

```>:params.toml
enableBreadcrumb = true
```

{{< expand "enableBreadcrumb" >}}
  ![Zdoc theme param - enableBreadcrumb](/images/configuration/zdoc/params.toml/11.enableBreadcrumb.png)
{{< /expand >}}

### enableBlogBreadcrumb

When false, breadcrumb will disappear on every blog post.

```>:params.toml
enableBlogBreadcrumb = true
```

{{< expand "enableBlogBreadcrumb" >}}
  ![Zdoc theme param - enableBlogBreadcrumb](/images/configuration/zdoc/params.toml/12.enableBlogBreadcrumb.png)
{{< /expand >}}

### enableEditBtn

When true, `EDIT THIS PAGE` button will appear on a page.

```>:params.toml
enableEditBtn = true
```

{{< expand "enableEditBtn" >}}
  ![Zdoc theme param - enableEditBtn](/images/configuration/zdoc/params.toml/13.enableEditBtn.png)
{{< /expand >}}

### enableToc

Hide/Show table of contents(TOC).

```>:params.toml
enableToc = true
```

{{< expand "enableToc" >}}
  ![Zdoc theme param - enableToc](/images/configuration/zdoc/params.toml/14.enableToc.png)
{{< /expand >}}

### enableMenu

Hide/Show menu sidebar.

```>:params.toml
enableMenu = true
```

{{< expand "enableMenu" >}}
  ![Zdoc theme param - enableMenu](/images/configuration/zdoc/params.toml/15.enableMenu.png)
{{< /expand >}}

### enableNavbar

Hide/Show navigation bar

```>:params.toml
enableNavbar = true
```

{{< expand "enableNavbar" >}}
  ![Zdoc theme param - enableNavbar](/images/configuration/zdoc/params.toml/16.enableNavbar.png)
{{< /expand >}}

### enableFooter

Hide/Show footer

```>:params.toml
enableFooter = true
```

{{< expand "enableFooter" >}}
  ![Zdoc theme param - enableFooter](/images/configuration/zdoc/params.toml/17.enableFooter.png)
{{< /expand >}}

### showPoweredBy

Hide/Show `poweredBy` text in the footer.

```>:params.toml
showPoweredBy = true
```

{{< expand "showPoweredBy" >}}
  ![Zdoc theme param - showPoweredBy](/images/configuration/zdoc/params.toml/18.showPoweredBy.png)
{{< /expand >}}

### paginateWindow

Setting it to 1 gives 7 buttons, 2 gives 9, etc. If set 1: [1 ... 4 5 6 ... 356] [1 2 3 4 5 ... 356] etc

```>:params.toml
paginateWindow = 1
```

### taxoPaginate

A number of elements per page on the blog tags page.

```>:params.toml
taxoPaginate = 5
```

### taxoGroupByDate

- "2006-01": group by month
- "2006": group by year

```>:params.toml
taxoGroupByDate = "2006"
```

### github

Link for the GitHub icon in the navigation bar

### enableComment

You can add a comment component to a blog type page. Supported comment services are

- utterances
