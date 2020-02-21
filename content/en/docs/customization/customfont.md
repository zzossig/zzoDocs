---
title: "Font"
date: 2020-01-30T15:40:17+09:00
draft: false
weight: 1
enableToc: false
---

## Using embeded font

1. Make a file at `root/data/font.toml`

    ```toml
    title_font = "\"Montserrat\", sans-serif"
    content_font = "\"muli\", sans-serif"
    ```

2. We have 6 embeded font

    - `"\"Montserrat\", sans-serif"`
    - `"\"Merriweather\", serif"`
    - `"\"muli\", sans-serif"`
    - `"\"Courgette\", cursive"`
    - `"\"Source Sans Pro\", sans-serif"`
    - `"\"League Gothic\", sans-serif"`

## Using custom css

1. Add custom css file

    ```toml
    ...
    custom_css = ["css/font.css"]
    ...
    ```

    `config/_default/params.toml`

    Set the above param and add file to assets/css/font.css

2. In your font.css file, add font-face something like this.

    ```css
    @font-face {
        font-family: 'Montserrat';
        src: url('../fonts/montserrat-black.woff2') format('woff2'),
            url('../fonts/montserrat-black.woff') format('woff');
        font-weight: 900;
        font-style: normal;
    }

    @font-face {
        font-family: 'Merriweather';
        src: url('../fonts/merriweather-regular.woff2') format('woff2'),
            url('../fonts/merriweather-regular.woff') format('woff');
        font-weight: 400;
        font-style: normal;
    }
    ```

3. Add your fonts file at root/static/fonts/myfont.xxx (If your url in step2 is ('../fonts/myfont.xxx')).

4. Make a font.toml file at root/data/font.toml and make variables as below.

    ```toml
    title_font = "\"Montserrat\", sans-serif"
    content_font = "\"Merriweather\", serif"
    ```

## Import google font

Make a file at `root/layouts/partials/head/custom-head.html` and then load font style. 

```html
<link href="https://fonts.googleapis.com/css?family=Noto+Sans+KR:400,700&display=swap&subset=korean" rel="stylesheet">
```