---
title: "Home Page"
date: 2020-10-20T15:05:06+09:00
draft: false
weight: 1
enableToc: true
---

{{< expand "Home Page Image" >}}
  ![Zdoc Home Page](/images/pages/zdoc/home-page.png)
{{</ expand >}}

You can decorate your homepage within a fixed frame. I made some front-matters for you to make it easy. 

At first, you should make `_index.md` file in the content root folder. (root/content/en/_index.md)

```root/content/en/_index.md
---
title: Z Themes
description: Hugo zzo, zdoc theme documentation home page
date: 2020-01-26T04:15:05+09:00
draft: false
...
---
```

## 1. Landing Page

{{< img src="/images/pages/zdoc/landing-page.png" title="Zdoc Landing Page" caption="Landing Page look and feel" alt="zdoc landing page">}}

You can set landing page Front-Matters like this. BackgroundImage Front-Matter is currently in development. Edit some Front-Matters by your self and find something useful on your own.

```root/content/en/_index.md
---
...
landing:
  height: 500
  image: favicon/android-icon-192x192.png
  title:
    - Z Themes
  text:
    - This is Hugo Z Themes documentation site
  titleColor:
  textColor:
  spaceBetweenTitleText: 25
  buttons:
    - link: zzo
      text: HUGO THEME ZZO
      color: primary
    - link: zdoc
      text: HUGO THEME ZDOC
      color: default
  # backgroundImage: 
  #   src: images/landscape.jpg
  #   height: 600
...
---
```

## 2. Banner Component

{{< img src="/images/pages/zdoc/banner.png" title="Zdoc Banner" caption="Banner component look and feel" alt="zdoc banner component">}}

```root/content/en/_index.md
---
...
updatesBanner: "Banner - &nbsp; [Hugo ZDoc theme](https://github.com/zzossig/hugo-theme-zdoc) &nbsp; just arrived"
...
---
```

## 3. Home Sections

{{< img src="/images/pages/zdoc/home-section-1.png" title="Zdoc Home section1" caption="Home section look and feel" alt="zdoc home section">}}
{{< img src="/images/pages/zdoc/home-section-2.png" title="Zdoc Home section2" caption="Home section look and feel" alt="zdoc home section">}}

You can add as many sections as you want. There are two types in home section.

- card
- normal

```root/content/en/_index.md
---
...
sections:
  - bgcolor: teal
    type: card
    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce id eleifend erat. Integer eget mattis augue. Suspendisse semper laoreet tortor sed convallis. Nulla ac euismod lorem"
    header: 
      title: Why Zdoc
      hlcolor: "#8bc34a"
      color: '#fff'
      fontSize: 32
      width: 220
    cards:
      - subtitle: Performance
        subtitlePosition: center
        description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce id eleifend erat. Integer eget mattis augue."
        image: images/section/keyboard.png
        color: white
        button: 
          name: Naver
          link: https://naver.com
          size: large
          target: _blank
          color: 'white'
          bgcolor: '#283593'
      - subtitle: Reliability
        subtitlePosition: center
        description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce id eleifend erat. Integer eget mattis augue. Suspendisse semper laoreet tortor sed convallis. Nulla ac euismod lorem"
        image: images/section/processor.png
        color: white
        button: 
          name: Google
          link: https://google.com
          size: large
          target: _blank
          color: 'white'
          bgcolor: '#283593'
      - subtitle: Productivity
        subtitlePosition: center
        description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce id eleifend erat. Integer eget mattis augue. Suspendisse semper laoreet tortor sed convallis. Nulla ac euismod lorem"
        image: images/section/root-server.png
        color: white
        button: 
          name: Yahoo
          link: https://yahoo.com
          size: large
          target: _blank
          color: 'white'
          bgcolor: '#283593'
  - bgcolor: DarkSlateBlue
    type: normal
    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce id eleifend erat. Integer eget mattis augue. Suspendisse semper laoreet tortor sed convallis. Nulla ac euismod lorem"
    header:
      title: Build it with Zdoc
      hlcolor: DarkKhaki
      color: "#fff"
      fontSize: 32
      width: 340
    body:
      subtitle: Extensible and customizable.
      subtitlePosition: left
      description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce id eleifend erat. Integer eget mattis augue. Suspendisse semper laoreet tortor sed convallis. Nulla ac euismod lorem"
      color: white
      image: images/section/root-server.png
      imagePosition: left
...
---
```

## 4. Home Footer

{{< img src="/images/pages/zdoc/home-footer.png" title="Zdoc Home Footer" caption="Home footer look and feel" alt="zdoc home footer">}}

```root/content/en/_index.md
---
...
footer:
  sections:
    - title: General
      links:
        - title: Docs
          link: https://gohugo.io/
        - title: Learn
          link: https://gohugo.io/
        - title: Showcase
          link: https://gohugo.io/
        - title: Blog
          link: https://gohugo.io/
    - title: resources
      links:
        - title: GitHub
          link: https://gohugo.io/
        - title: Releases
          link: https://gohugo.io/
        - title: Spectrum
          link: https://gohugo.io/
        - title: Telemetry
          link: https://gohugo.io/
    - title: Features
      links:
        - title: GitHub
          link: https://gohugo.io/
        - title: Releases
          link: https://gohugo.io/
        - title: Spectrum
          link: https://gohugo.io/
        - title: Telemetry
          link: https://gohugo.io/
  contents: 
    align: left
    applySinglePageCss: false
    markdown:
      |
      ## Zzo docs
      Copyright © 2020. All rights reserved.
...
---
```