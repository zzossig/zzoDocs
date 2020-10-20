---
title: "Code"
date: 2020-10-20T19:19:37+09:00
draft: false
weight: 4
enableToc: false
---

code / codes => Tabbed code-block. indentation matters.

## 1. How to use

`````
{{</* codes java javascript */>}}
  {{</* code */>}}
  ```java
  System.out.println('Hello World!');
  ```
  {{</* /code */>}}
  {{</* code */>}}
  ```javascript
  console.log('Hello World!');
  ```
  {{</* /code */>}}
{{</* /codes */>}}
`````

## 2. What it looks like

{{< codes java javascript >}}
  {{< code >}}
  ```java
  System.out.println('Hello World!');
  ```
  {{< /code >}}
  {{< code >}}
  ```javascript
  console.log('Hello World!');
  ```
  {{< /code >}}
{{< /codes >}}