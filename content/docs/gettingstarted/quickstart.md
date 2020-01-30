---
title: "Quick Start"
date: 2020-01-30T10:16:47+09:00
description:
draft: false
weight: -1
enableToc: false
---

If you don't want to think of anything but want to get a working blog, do this. This guide assumes that you already installed the Hugo-extended version

1. Make a folder that will contain the blog source code.
2. Go to the folder directory you made in step 1, and create a new Hugo site by typing 

    ```
    hugo new site .
    ```

    Keep in mind that there is a `.` at the end.
3. Download the [hugo-theme-zzo](https://github.com/zzossig/hugo-theme-zzo) repository. I recommend to use `submodule` , but this is just a quick start guide.
4. Make the `zzo` folder in the themes folder and unzip the downloaded repository to the folder(root/themes/zzo).
5. In the zzo folder you made, you can see the exampleSite folder. There are four folders inside the folder(config, content, resources, static). Just copy-paste them to your project root folder. (delete overlapping folders before you do this)
6. Now, you are good to go. Run Hugo by typing `hugo server` at your root directory.
