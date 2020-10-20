---
title: "Quick Start"
date: 2020-01-30T10:16:47+09:00
description:
draft: false
weight: -1
---

If you don't want to think about anything but want to get a working blog, do this. This guide assumes that you already have installed the [Hugo-extended](https://gohugo.io/getting-started/installing/) version

1. Make a folder that will contain the blog source code. (For example: c:\\workspace\\quickstartblog)
2. Go to the folder directory you made in step 1(`quickstartblog` in my case), and create a new Hugo site by typing 

    ```
    hugo new site .
    ```

    Keep in mind that there is a `.` at the end.
3. Download the [hugo-theme-zzo](https://github.com/zzossig/hugo-theme-zzo) repository. I recommend to use `submodule` , but this is just a quick start guide. Download the repository is easier than using the git submodule.
4. Make a `zzo` folder in your blog themes folder. (`quickstartblog/themes/zzo` in my case)
5. Unzip the zzo repository to your zzo folder
6. In the zzo folder, you can see the exampleSite folder. There are four folders inside (config, content, resources, static). Just copy-paste them to your project root folder. (delete overlapping folders or just override the folders)
7. Now, you are good to go. Run Hugo by typing `hugo server` at your root directory.
