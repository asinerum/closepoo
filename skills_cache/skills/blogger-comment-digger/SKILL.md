---
name: blogger-comment-digger
description: Download (a.k.a dig, or retrieve) users comments from a public Blogger blog and save them to an HTML file
---

# blogger comment download/dig/retrieve

> **PREREQUISITE:** Run `npm i bloggerize` to install required Node JS library, and clone https://github.com/asinerum/bloggerize for sample scripts

Target: Download/Dig/Retrieve comments from blog URL

## Usage

### Use case 1: Download comments in 3 pages from page 21, posted between Oct 6th 2014 and Nov 30th 2014, of a public blog <URL>

```bash
node download2.js pages:3,page:21,from:2014-10-06,to:2014-11-30,url:<URL>
```

Command argument-list can be put in quotes:

```bash
node download2.js "pages:3,page:21,from:2014-10-06,to:2014-11-30"
```

For general cases:

```bash
node download2.js pages:<PAGES>,page:<PAGE>,from:<DATE_BEGIN>,to:<DATE_END>,url:<URL>
```

### Use case 2: Download a certain user's comments

In this case, a valid User ID <UID> must be provided by user himself, for example "08901517722071939298" or something similar.

```bash
node download2.js "pages:<PAGES>,page:<PAGE>,from:<DATE_BEGIN>,to:<DATE_END>,url:<URL>,pte:<UID>"
```

## Arguments value and mandatoriness

| Argument   | Required | Default | Description |
|------------|----------|---------|-------------|
| DATE_BEGIN | yes      | -       | Start date  |
| DATE_END   | yes      | -       | End date    |
| PAGES      | no       | 1       | Total pages |
| PAGE       | no       | 1       | From page   |
| URL        | no       | empty   | Blog URL    |
| UID        | no       | empty   | User ID     |

- Arguments DATE_BEGIN and DATE_END are mandatory, and must be formatted as "2006-01-02" (RFC3339 style) or "2/1/2006" (UK style).
- Arguments URL and UID are not mandatory. If they were missing, just ignore them (let them be empty).
