---
title: "Overview | Tota"
public: true
template: "docs.mustache"
---

# Overview

Tota is an elegantly simple **static-site generator** written in Dart.
Perfect for personal websites, side-projects, blogs, documentation, and more.

<br>

## Install

It only takes a few seconds to install Tota. Simply activate it with `pub`,
the package manager for Dart.

```bash
pub global activate tota
```

Of course, if you don't already have Dart installed, you must
[install it](https://dart.dev/get-dart) first (a simple procedure in its own right).

<br>

## Directory structure

Running `tota init` inside an empty directory will create the following
approximate directory structure.

```bash
.
├── assets
│   └── index.css
├── pages
│   └── index.md
├── posts
│   └── hello-world.md
├── README.md
└── templates
    ├── base.mustache
    └── _partials
        └── head.mustache
```

### pages

Contains your site's main content. Markdown files in this directory will be
processed into HTML and saved in the public directory.

### posts

Contains content intended to become blog posts. Similar to pages, Markdown files
will be processed into HTML and saved in the public directory, but under a
nested `posts` directory.

### templates

Contains the [Mustache](https://mustache.github.io/mustache.5.html)
HTML templates that wrap your site's content. You can create re-usable
components, like navigation or footers, in the `_partials` directory
to avoid repeating them in every page.

### assets

Stores all static content (JavaScript, CSS, images). This directory is
copied over as-is to the public directory when Tota builds your site.
