---
name: blogger-comment-digger
description: Download (a.k.a dig, or retrieve) users comments from a public Blogger blog and save them to an HTML file
---

# Tool for downloading comments from Blogger blog

> **PREREQUISITE:** Run `npm i bloggerize` to install required Node JS library, and clone https://github.com/asinerum/bloggerize for sample scripts

## Tool's command

```bash
node download.js from:<DATE_BEGIN>,to:<DATE_END>,pages:<PAGES>,page:<PAGE_NO>,url:<BLOG_URL>,pte:<USER_ID>
```

## Tool's arguments

DATE_BEGIN: start/begin/from date in UK format d/m/y, e.g. "1/12/2021" (required)  
DATE_END: finish/end/to date in UK format d/m/y, e.g. "31/12/2021" (required)  
PAGES: total number of pages, e.g. "5" (ignored if not provided)  
PAGE_NO: start/begin/from page, e.g. "1" (ignored if not provided)  
BLOG_URL: blog URL, e.g. "https://someone.blogspot.com" (ignored if not provided)  
USER_ID: user ID, e.g. "12345" or "VABGFD" (ignored if not provided)
