---
title: "Font"
date: 2020-01-30T15:40:17+09:00
draft: false
weight: 1
enableToc: false
---

## Using embeded font

This theme already has the 6 different fonts. You can use any of these fonts. To do that:

1. Make a file at `root/data/font.toml` with following params

    ```toml
    title_font = "\"Montserrat\", sans-serif"
    content_font = "\"muli\", sans-serif"
    ```

2. Here is the list of 6 fonts that are avalable 

    - `"\"Montserrat\", sans-serif"`
    - `"\"Merriweather\", serif"`
    - `"\"muli\", sans-serif"`
    - `"\"Courgette\", cursive"`
    - `"\"Source Sans Pro\", sans-serif"`
    - `"\"League Gothic\", sans-serif"`

## Using custom font

If you want to use any fonts which are not listed above, you can do so. There are 2 ways to do this. 

#### Method 1

If you have the font files (e.g. .woff2 or .woff) follow the instructions in this section.

#### Method 2

If your custom font is from Google fonts, you can skip this section (adding font files) & follow the instructions in the next section to add link to your Google font.

1. Add a custom css file first

    ```toml
    ...
    custom_css = ["css/font.css"]
    ...
    ```

   
    Set the above param in `config/_default/params.toml` and then add the file to assets/css/font.css

2. In your font.css file, add the custom font-face in a format like this.

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

3. Add your font files at `root/static/fonts/myfont.xxx` (assuming your url in step2 is ('../fonts/myfont.xxx')). In case your custom font is from Google Fonts you need not add the font files, instead you can just add the link tag in `root/layouts/partials/head/custom-head.html` (complete description is given below). 

4. Make a font.toml file at root/data/font.toml and make variables as below.

    ```toml
    title_font = "\"Montserrat\", sans-serif"
    content_font = "\"Merriweather\", serif"
    ```

## Using fonts from Google fonts (as custom font)

If the custom font that you wish to use is available on Google Fonts, then you need not provide the font files (as mentioned in the previous step). Instead you can add the link to the specific Googlefont by following the steps below.

Make a file at `root/layouts/partials/head/custom-head.html` and then load font style. 

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<!-- Replace the next line with your font's link -->
<link href="https://fonts.googleapis.com/css?family=Noto+Sans+KR:400,700&display=swap&subset=korean" rel="stylesheet">
```
