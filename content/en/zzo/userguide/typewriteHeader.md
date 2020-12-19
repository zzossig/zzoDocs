---
title: "Typewrite Header"
date: 2020-10-21T09:09:18+09:00
draft: false
weight: 11
enableToc: false
---

You can set a typewriter header that appears on your home page. Follow the steps below.

1. Set the `homeHeaderType` param to `typewriter` in the `params.toml` file.
    ```params.toml
    ...
    homeHeaderType = "typewriter" # text, img, slide, typewriter
    ...
    ```
2. Add some Front-Matters in your content root `_index.md` file.
    ```_index.md
    ---
    header:
      - type: typewriter
        methods:
          - typeString: Hello world!
          - pauseFor: 2500
          - deleteAll: true
          - typeString: Strings can be removed
          - pauseFor: 2500
          - deleteChars: 7
          - typeString: <strong>altered!</strong>
          - pauseFor: 2500
        options:
          loop: true
          autoStart: false
        height: 190
        paddingX: 50
        align: center
        fontSize: 44
        fontColor: yellow
    ...
    ---
    ```
3. In the above, you can see the methods, options Front-Matter. Refer the [typewriterjs](https://safi.me.uk/typewriterjs/) site. Change it to your taste