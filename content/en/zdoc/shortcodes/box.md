---
title: "Box"
date: 2020-10-20T19:10:25+09:00
draft: false
weight: 2
enableToc: false
---

## 1. How to use

- Markdownify box

    ```
    {{</* boxmd */>}}
    Some markdown contents
    {{</* /boxmd */>}}
    ```

- Simple box

    ```
    {{</* box */>}}
    Some contents
    {{</* /box */>}}
    ```

## 2. What it looks like

{{< boxmd >}}
*You* can use ***markdown*** **syntax** `here`.
1. box
2. boxmd
{{< /boxmd >}}

{{< box >}}
Plain Text
{{< /box >}}