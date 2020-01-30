---
title: "Gallery Page"
date: 2020-01-30T12:45:41+09:00
draft: false
weight: 1
enableToc: false
---

There are two modes to the gallery. You can specify it in the front matter.

content/gallery/anygalleryname/index.md

```yaml

---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
description: my gallery
type: gallery
mode: one-by-one # at-once or one-by-one
tags:
-
series:
-
categories:
-
images: # when mode is one-by-one, images front-matter variable works
  - image: image1.jpg
    caption: caption1
  - image: image2.jpg
    caption: caption2
    ...
---

```

## one-by-one

If you set the mode to one-by-one, you have to set the `images` front matter. This mode is used to specify captions, order of images.

```yaml
---
...
images: # when mode is one-by-one, images front-matter variable works
  - image: image1.jpg
    caption: caption1
  - image: image2.jpg
    caption: caption2
    ...
```

## at-once

If you set the mode to at-once, you don't need to set the `images` front-matter. Just put all your images to the static/gallery/anygalleryname folder.

1. Make a gallery folder under the content folder

    ```
    root
    ├── content
    │   ├── gallery
    ```

2. Make a sub folder under the gallery folder

    ```
    root
    ├── content
    │   ├── gallery
    │   │   ├── anygalleryname
    ```

3. Make a index.md file under the sub folder using this command

    ```
    hugo new --kind gallery gallery/anygalleryname/index.md
    ```

4. Put your images in static folder

    ```
    root
    ├── static
    │   ├── gallery
    │   │   ├── anygalleryname
    │   │   │   ├── ...your images here
    ```