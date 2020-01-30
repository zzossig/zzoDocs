---
title: "Katex"
date: 2020-01-30T10:27:06+09:00
draft: false
weight: 3
enableToc: false
---

`````
---
title:
date:
description:
...
libraries:
- katex
---

The following

$$ \int_{a}^{b} x^2 dx $$

Is an integral

$$ \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } $$

Enable Katex in the config file by setting the `katex` param to `true`. This will import the necessary Katex CSS/JS. 

See the online reference of [supported TeX functions](https://katex.org/docs/supported.html). 

**Note:** For inline math to render correctly, your content file extension must be `.mmark`. See the [official mmark site](https://mmark.nl/). 

```
Inline math: $ \varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887… $
```

Inline math: $ \varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887… $

```
Block math:

$$ \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } $$
```

Block math:

$$ \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } $$
`````