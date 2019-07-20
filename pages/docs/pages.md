---
title: "Pages | Tota"
template: "docs"
public: true
---

# Pages

The most basic type of resource, usually devoid of any dates, and suitable for home pages, landing pages, and other standalone site pages.

<br>

## Pages directory

Pages are written in Markdown (`.md`) format and stored in the pages directory. Tota will convert these files to HTML and save them in the `public` directory when your site is built.

The pages directory location can be changed in the directory [configuration](/docs/configuration#directory).

```bash
TOTA_PAGES_DIR="pages"
```

<br>

## Create a page

Create a new page by running the [new command](/docs/commands/#new). This will create a new Markdown file in the pages directory.

```bash
tota new "Parrots and Cockatoos"
```

Alternatively, you can manually create files in the pages directory.

<br>

## Filenames

By default, the `new` command will transform your page title into a [slug](https://en.wikipedia.org/wiki/Clean_URL#Slug) and use that as the filename. For example, the command from the example above will produce the file:

```bash
pages/parrots-and-cockatoos.md
```

⚠️ Filename are important! They are re-used for the HTML files and therefore reflected in the URL.
Make sure your filenames are URL-friendly and don't contain unsafe characters
like spaces and punctuation marks.

<br>

## Sub-directories

You can group related pages into sub-directories within the pages directory. The same directory structure will be re-used in the `public` directory when Tota builds your site.

This allows you to create a nested URL structure:

```http
https://www.example.com/birds/psittaciformes/parrot.html
```

<br>

## See also

- [Posts](/docs/posts)
- [Front matter](/docs/front-matter)
- [Templates](/docs/templates)

<br>
