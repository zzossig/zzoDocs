---
title: "Codeblock"
date: 2020-10-21T08:19:01+09:00
draft: false
weight: 4
enableToc: false
---

## Normal usage of code block

````
```javascript
console.log('Hello World!');
```
````

## You can set the code-block title and line number to $, > symbol.

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

## You could also do this.

````
```javascript:etc/dir/myscript.js
console.log('Hello World!');
```
````

```javascript:etc/dir/myscript.js
console.log('Hello World!');
```

Just keep in mind that the code block title should end with extensions. (e.g: `.js`, `.c`, `.python`) otherwise, the code-block would not render properly

## We have a code-tab shortcode

Make it easy to switch between different code

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

````
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
````