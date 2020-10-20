---
title: "CSS"
date: 2020-01-30T15:39:37+09:00
draft: false
weight: 5
enableToc: false
---

1. Add this line of code to your params.toml file.

    ```toml
    ...
    custom_css = ["css/custom.css", "scss/custom.scss", ...]
    ...
    ```

    `config/_default/params.toml`

2. Add your file to assets folder. Filename must match with config params you set above.

    ```
    assets/scss/custom.scss
    assets/css/custom.css
    ```

3. If you want to modify the Zzo theme's default color, you should override the theme style. For example, if you're going to change the body background-color because I set the background-color in #body selector, not in the body tag selector, you should override body background-color there. Body tag selector won't work. And make sure to set !important. After setting the values, restart Hugo.

    ```css
    

    ...
    #body {
      background-color: red !important;
    }
    ...
    ```

    `assets/scss/custom.scss` or `assets/css/custom.css`