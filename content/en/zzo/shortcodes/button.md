---
title: "Button"
date: 2020-02-02T03:00:00+09:00
draft: false
weight: 9
enableToc: false
---

* Simple button

    `````
    {{</* button href="https://..." */>}}button{{</* /button */>}}
    `````

* You can specify width, height

    `````
    {{</* button href="https://..." width="100px" height="36px" */>}}button{{</* /button */>}}
    `````

* Set color

    `````
    {{</* button href="https://..." width="100px" height="36px" color="primary" */>}}button{{</* /button */>}}
    `````

    You can customize the button primary color in the file at `root/data/button.toml`. Just copy-paste the theme's button.toml file and edit the params as you want.

    ```toml
    # restart hugo after set the values
    dark_primary_color = "#82aaff"
    light_primary_color = "#728fcb"
    hacker_primary_color = "#cddc39"
    solarized_primary_color = "#689f38"
    kimbie_primary_color = "#8ab1b0"
    ```

    `button.toml`