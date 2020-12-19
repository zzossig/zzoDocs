---
title: "Contact Page"
date: 2020-01-30T12:49:57+09:00
draft: false
weight: 2
enableToc: false
---

{{< expand "Netlify Form" >}}

#### 1. Make a file at root/content/contact/index.md

```yaml
---
title: "Contact Me"
description: Contact page
type: contact
service: netlifyform
recaptcha: true
redirect-after-submit: "/redirect"
---

Thanks for choosing to reach out! I will get back to you shortly.
```

In the front-matter, you can see 2 options.
One is recaptcha, and the other is redirect.
For using **recaptcha**, just set it to true.
For using the **redirect** option, set the `redirect-after-submit` to your redirection url.
And then you need to prepare a page for that redirection url.

#### 2. Create a folder at root/content/redirect

I use the folder name to redirect because I set the redirection url to `/redirect`

#### 3. Create a file at root/content/redirect/index.md

```yaml
---
title: "Thanks for your submission"
type: about
---

{{</* custombox */>}}
## Thank you for sparing time to reach out.<br/> We shall be in touch with you shortly.
{{</*/ custombox */>}}
```

This file is a contents markdown file that people see after redirection.
I set the type to `about` because about page is an empty page and it is best fits for redirection contents.

#### 4. Add contact menu at root/config/_default/menus.en.toml.

```toml
...
[[main]]
  identifier = "contact"
  name = "contact"
  url = "contact"
  weight = 6
```

{{< /expand >}}

{{< expand "Getform" >}}

#### 1. Make a file at root/content/contact/index.md

```yaml
---
title: "Contact"
description: Contact page
type: contact
service: getform
getformToken: "yourformtoken"
---

This is contact page.
```

#### 2. Add contact menu at root/config/_default/menus.en.toml.

```toml
...
[[main]]
  identifier = "contact"
  name = "contact"
  url = "contact"
  weight = 6
```

{{< /expand >}}

{{< expand "Formspree" >}}

#### 1. Make a file at root/content/contact/index.md

```yaml
---
title: "Contact"
description: Contact page
type: contact
service: formspree
formId: "your@email.com"
---

This is contact page.
```

#### 2. Add contact menu at root/config/_default/menus.en.toml.

```toml
...
[[main]]
  identifier = "contact"
  name = "contact"
  url = "contact"
  weight = 6
```

{{< /expand >}}

## default

If you want just a blank page and use a markdown, set the service param empty.
