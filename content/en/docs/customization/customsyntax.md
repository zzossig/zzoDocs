---
title: "Syntax Highlight"
date: 2020-01-30T15:39:43+09:00
draft: false
weight: 3
enableToc: false
---

1. Make a file at `root/data/skin.toml`. We can set the code block color theme by theme

    ```toml
    # https://xyproto.github.io/splash/docs/longer/all.html
    # restart hugo after change this value
    theme_light_chroma = "default"
    theme_dark_chroma = "default"
    theme_hacker_chroma = "default"
    theme_solarized_chroma = "default"
    theme_kimbie_chroma = "default"

    # possible value: default, dark, light, hacker, solarized, kimbie
    # restart hugo after change this value
    theme_light_chroma_background = "default"
    theme_dark_chroma_background = "default"
    theme_hacker_chroma_background = "default"
    theme_solarized_chroma_background = "default"
    theme_kimbie_chroma_background = "default"
    ```

    `skin.toml`

2. Set the theme_dark_chroma, theme_light_chroma, ... params value as you want. Refer this [link](https://xyproto.github.io/splash/docs/all.html). If theme_[xxxx]_chroma value include - or _ like special character, just delete it.
For example, if you want use solarized-dark256 style, set the param like this.

    ```
    theme_dark_chroma = "solarizeddark256"
    ```

    `root/data/skin.toml`

3. Set the theme_dark_chroma_background, theme_light_chroma_background, ... params value to one of the following values.

    `default` `dark` `light` `hacker` `solarized` `kimbie`