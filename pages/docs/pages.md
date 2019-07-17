---
title: "Pages | Tota"
template: "docs"
public: true
---

# Pages

The most basic type of resource, usually devoid of any dates, and suitable for home pages, landing pages, and other standalone site pages.

Pages are written in Markdown and are stored in the pages directory, which is set by the `TOTA_PAGES_DIR` configuration setting. The Markdown file is converted to HTML when Tota builds your site.

<br>

## Create a page

Create a new page by running the [new command](/docs/commands/#new). This will create a new Markdown file in the pages directory.

```bash
tota new "Example page"
```

Alternatively, you can manually create files in the directory.

<br>

## Filenames

By default, the `new` command will convert your page title into a [slug](https://en.wikipedia.org/wiki/Clean_URL#Slug) and use that as the filename. For example, the command from above will produce the file:

```bash
pages/example-page.md
```

⚠️ The filename is reused for the generated HTML file, so if you prefer to manually create pages, ensure your filenames are URL-friendly and don't contain unsafe characters like spaces and punctuation marks.

<br>

## Sub-directories

You can group related pages into sub-directories within the pages directory. The same directory structure will be re-used in the `public` directory when Tota builds your site.

<br>