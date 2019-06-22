---
title: "Configuration | Tota"
public: true
template: "docs.mustache"
---

# Configuration

Tota uses environment variables prefixed with `TOTA_*` for all settings.
You can modify these settings with a `.env` (dotenv) file placed in the
project directory.

<br>

## Site

Name | Description
--- | ---
`TOTA_TITLE` | The title of the website.
`TOTA_DESCRIPTION` | Short description of the website.
`TOTA_AUTHOR` | The website author's name.
`TOTA_LANGUAGE` | The language of the website in [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format. Default is `en`.

<br>
<br>

## Directory
Name | Description
--- | ---
`TOTA_PUBLIC_DIR` | Contains all generated and publicly-accessible files.
`TOTA_PAGES_DIR` | Contains the source files for pages.
`TOTA_POSTS_DIR` | Contains the source files for posts. Also used in the URL as the blog sub-directory.
`TOTA_TEMPLATES_DIR` | Contains the [mustache](https://mustache.github.io/mustache.5.html) HTML template files.
`TOTA_ASSETS_DIR` | Contains non-page static files (JavaScript, CSS, etc.)

<br>
<br>

## Default `.env` file

Tota ships with the following dotenv file as default. If you ever misplace it,
you can create a new copy from below.

```bash
# Title of the website.
TOTA_TITLE="Tota"

# Short description of the website.
TOTA_DESCRIPTION="Tota is a simple, elegant framework for generating static sites."

# The website author's name.
TOTA_AUTHOR="Tota team"

# The language of the website in ISO 639-1 format. Default is `en`.
TOTA_LANGUAGE="en"

  # Contains all generated and publicly-accessible files.
TOTA_PUBLIC_DIR="public"

# Contains the source files for pages.
TOTA_PAGES_DIR="pages"

# Contains the source files for posts. Also used in the URL as the blog directory.
TOTA_POSTS_DIR="posts"

# Contains the mustache HTML template files.
TOTA_TEMPLATES_DIR="templates"

# Contains non-page static files (JavaScript, CSS, etc.)
TOTA_ASSETS_DIR="assets"
```
