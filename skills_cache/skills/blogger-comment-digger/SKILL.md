---
name: blogger-comment-digger
description: Download (a.k.a dig, or retrieve) users comments from a public Blogger blog and save them to an HTML file
---

# Tool for downloading comments from Blogger blog

> **PREREQUISITE:** Run `npm i bloggerize` to install required Node JS library, and clone https://github.com/asinerum/bloggerize for "download.js" and other required scripts.

## Tool's command

```bash
node download.js "from:<DATE_BEGIN>,to:<DATE_END>,pages:<PAGES>,page:<PAGE_NO>,url:<BLOG_URL>,pte:<USER_ID>"
```

## Tool's parameters (do not ask about the parameters if they are not provided)

- DATE_BEGIN: starting/beginning date (a date-string in UK format d/m/y), blank by default (a.k.a current month).
- DATE_END: finishing/ending date (a date-string in UK format d/m/y), blank by default (a.k.a current day).
- PAGES: total number of pages (an integer number), 1 by default.
- PAGE_NO: starting/beginning page (an integer number), 1 by default.
- BLOG_URL: blog URL (an URL string), "https://an-hoang-trung-tuong-2014.blogspot.com" by default.
- USER_ID: user ID (a string or number), blank by default (a.k.a everyone).
