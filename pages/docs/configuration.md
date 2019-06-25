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

The HTML tags in `<head>` will be populated from this config.

Name | Description
--- | ---
`TOTA_URL` | The website URL (protocol and domain).
`TOTA_TITLE` | The title of the website.
`TOTA_DESCRIPTION` | Short description of the website.
`TOTA_AUTHOR` | The default post author.
`TOTA_LANGUAGE` | The language of the website in [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format. Default is `en`.

<br>
<br>

## Directory

You are permitted to choose your own directory names in your Tota project,
as long as you update the following settings.

Name | Description
--- | ---
`TOTA_PUBLIC_DIR` | Contains all generated and publicly-accessible files.
`TOTA_PAGES_DIR` | Contains the source files for pages.
`TOTA_POSTS_DIR` | Contains the source files for posts. Also used in the URL as the blog sub-directory.
`TOTA_TEMPLATES_DIR` | Contains the [mustache](https://mustache.github.io/mustache.5.html) HTML template files.
`TOTA_ASSETS_DIR` | Contains non-page static files (JavaScript, CSS, etc.)

<br>
<br>

## Deploy

These settings are used to manage deployments.

Name | Description
--- | ---
`TOTA_NETLIFY_SITE` | The name of the site on Netlify.
`TOTA_NETLIFY_TOKEN` | Netlify personal access token.

<br>
<br>

## Default `.env` file

Tota ships with the following dotenv file as default. If you ever misplace it,
you can create a new copy from below.

```bash
# The website URL (protocol and domain).
TOTA_URL="https://tota.dev"

# Title of the website.
TOTA_TITLE="Tota"

# Short description of the website.
TOTA_DESCRIPTION="Tota is a simple, elegant framework for generating static sites."

# The default post author.
TOTA_AUTHOR="izolate"

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

# The name of the site on Netlify.
TOTA_NETLIFY_SITE=""

# Netlify personal access token.
TOTA_NETLIFY_TOKEN=""
```
