---
title: "Publication Page"
date: 2020-02-08T19:07:57+09:00
draft: false
weight: 6
enableToc: false
---

Basially, the publication page is created to represent a `.bib` file. But you can use the publication page as needed.

## using zzo-bibtex-parer

I made a library to parse the `.bib`file to `md`file. Follow the steps below to install the library.

1. Install pip(The Python Package Installer) first.

2. Install `zzo-bibtex-paresr` by typing this in your terminal.
    ```
    pip install zzo-bibtex-parser==1.0.8
    ```

3. Prepare your .bib file to the root folder.

4. Assuming your file name is bibtex.bib, from the root of your project, type this.
    ```
    zzo --path bibtex.bib
    ```

5. Make a publication menu. In your menu.toml file
    ```
    ...
    [[main]]
      identifier = "publication"
      name = "Publications"
      url = "publication"
      weight = 6
    ```

6. Set new param to your `params.toml` file.
    ```
    ...
    pubPaginate = 20
    ```

7. Now, you can see the publications page when you start the hugo

8. If the year of the post is the curreny year, the post set the `pinned` param to `true` by default.

## manually

If you don't have `.bib` file and just take advantage of the publication page, you can manually make the pages.

1. Make a publication folder in content folder. `root/content/publication`
2. Make a subfolder and `_index.md` file. This subfolder will be a section of the publication page. I'll make an `article` folder as an example.

    `root/content/publication/article/_index.md`

    ```yaml
    ---
    title: article # must be the same with the folder name
    date: 2020-02-08 19:37:21.760316
    description: Publication - article # for SEO
    ---
    ```

3. Make a folder in the article folder we made above and make `index.md` file in that folder.

    `root/content/publication/article/american_libraries_magazine/index.md`
    
    ```yaml
    ---
    authors: ['Watson, Brian M.']
    publication: "American Libraries Magazine"
    abstract: "Kristin Pekoll, Assistant Director of ALA Office for Intellectual Freedom (OIF) began the session by announcing that OIF had recorded 531 affected items in 2018—which is a step beyond just challenges. These items included books films, board games, video games, magazines and much more. Sarah Ward, outreach librarian at Hunter College Libraries in New York … Continue reading Still Chilling: Censorship Beyond Banned Books →"
    links:
    - name: url
      link: https://americanlibrariesmagazine.org/blogs/the-scoop/still-chilling-censorship-beyond-banned-books/)
    shorttitle: "Still Chilling"
    copyright: "All rights reserved"
    title: "Still Chilling: Censorship Beyond Banned Books"
    ENTRYTYPE: "article"
    enableToc: False
    enableWhoami: True
    pinned: False
    publishDate: "2019-06-01"
    ---
    ```

4. In the above `yaml` file, the `ENTRYTYPE` param should be the same with the section name(In our case, `article`).

5. Now, you get the idea. Make any section you want and there, make any publication like above.

6. You can pin the publication by setting parameter `pinned` to `true`. The pinned publication will show up in the overview page. 