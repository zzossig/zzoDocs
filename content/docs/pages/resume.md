---
title: "Resume Page"
date: 2020-02-10T10:01:01+09:00
draft: false
weight: 7
enableToc: false
---

Follow the below steps to make a resume page.

1. Make a folder and file at `root/content/resume/index.md`

    {{< expand "index.md" >}}

    ```yaml
    ---
    title: "Resume"
    date: 2020-02-09T20:13:59+09:00
    description: My awesome resume
    type: resume
    enableToc: false
    header:
      image: 
        src: images/whoami/avatar.png
        height: 100
        alt: resume image
      infos:
        name: choi
        email: cshl0ve@naver.com
        phone: 000-0000-0000
        website: https://www.exampleSite.com
        addr: my address
    items:
      - title: myTitle
        sections:
          - title: sectionTitle1
            subtitle: sectionSubtitle1
            startDate: 2020-02-09T20:13:59+09:00
            endDateText: current
            endDate: 2020-02-10T20:13:59+09:00
            contents: | 
              # h1
              ## h2
              ### h3
              1. hele
              2. dasg
              3. 125
              - bbb
              - eee
              - qqq
              > asdignasg

              [heeeee](https://google.com)

          - title: sectionTitle2
            subtitle: sectionSubtitle2
            date: 2020-02-07T20:13:59+09:00
            contents: | 
              Describe your role here lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo.

              Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
          - title: sectionTitle3
            subtitle: sectionSubtitle3
            date: 2020-02-05T20:13:59+09:00
            contents: | 
            
      - title: myTitle2
        sections:
          - title: sectionTitle2-1
            subtitle: sectionSubtitle2-1
            date: 2020-02-09T20:13:59+09:00
            contents: | 
            
          - title: sectionTitle2-2
            subtitle: sectionSubtitle2-2
            date: 2020-02-07T20:13:59+09:00
            contents: | 
            
          - title: sectionTitle2-3
            subtitle: sectionSubtitle2-3
            date: 2020-02-05T20:13:59+09:00
            contents: | 
    ---
    ```
    {{< /expand >}}
    
3. Edit the params to yours. Leave the params empty or delete if you don't want to set the params.

4. Be careful that the `contents` param accept a markdown syntax. It should start with `|` and a value should one level more deep than it's key(`contents`)

5. You can set as many items as you want.
    
    ```yaml
    ...
    items:
      - title
        sections:
      - title:
        sections:
        ...
    ```

6. finally, make a menu in your `menu.toml` file.

    ```toml
    ...
    [[main]]
      identifier = "resume"
      name = "whatever"
      url = "resume"
      weight = 6
    ```