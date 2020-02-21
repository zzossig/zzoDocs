---
title: "Codeblock"
date: 2020-02-09T17:43:01+09:00
draft: false
weight: 8
enableToc: false
---

You should reference the official site documentation. [https://gohugo.io/content-management/syntax-highlighting/](https://gohugo.io/content-management/syntax-highlighting/)


- Normal usage of code block
    ````
    ```javascript
    console.log('Hello World!');
    ```
    ````

- You can set the code-block title and line number to `$`, `>` symbol.

    ````
    ```>:s22adg.sh
    agasgas
    ```

    ```$:sadg.sh
    agasgas
    agasgas
    agasgas
    agasgas
    agasgas
    ```

    ```:/etc/profile.java
    System.out.println();
    ```
    ````
    {{< img src="/images/configuration/codeblock-with-title.png" title="Code Block" caption="with title, symbol line number" alt="code-block with title, symbol line number">}}

    You could also do this.
    ````
    ```javascript:etc/dir/myscript.js
    console.log('Hello World!');
    ```
    ````

Just keep in mind that the code block title should end with extensions. (e.g: `.js`, `.c`, `.python`) otherwise, the code-block would not render properly