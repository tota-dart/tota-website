---
title: "Configuration | Tota"
template: "docs"
public: true
---

# Configuration

While Tota ships with sensible defaults to allow for zero-configuration use, it also allows you to override settings by using environment variables prefixed with `TOTA_*`.

<br>

## Site

The HTML tags in `<head>` will be populated from this config.

| Name               | Description                                                                                                                |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------- |
| `TOTA_URL`         | The website URL (protocol and domain).                                                                                     |
| `TOTA_TITLE`       | The title of the website.                                                                                                  |
| `TOTA_DESCRIPTION` | Short description of the website.                                                                                          |
| `TOTA_AUTHOR`      | The default post author.                                                                                                   |
| `TOTA_LANGUAGE`    | The language of the website in [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format. Default is `en`. |

<br>
<br>

## Directory

You are permitted to choose your own directory names in your Tota project,
as long as you update the following settings.

| Name                 | Description                                                                              |
| -------------------- | ---------------------------------------------------------------------------------------- |
| `TOTA_PUBLIC_DIR`    | Contains all generated and publicly-accessible files.                                    |
| `TOTA_PAGES_DIR`     | Contains the source files for pages.                                                     |
| `TOTA_POSTS_DIR`     | Contains the source files for posts. Also used in the URL as the blog sub-directory.     |
| `TOTA_TEMPLATES_DIR` | Contains the [mustache](https://mustache.github.io/mustache.5.html) HTML template files. |
| `TOTA_ASSETS_DIR`    | Contains non-page static files (JavaScript, CSS, etc.)                                   |

<br>
<br>

## Posts

These settings relate only to posts.

| Name               | Description                                                                                                                                      | Default |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------- |
| `TOTA_DATE_FORMAT` | The date format. Read Dart's `intl` package [docs](https://pub.dev/documentation/intl/latest/intl/DateFormat-class.html) for formatting options. | `yMMMd` |

<br>
<br>

## Deploy

These settings are used to manage deployments.

| Name                 | Description                      |
| -------------------- | -------------------------------- |
| `TOTA_NETLIFY_SITE`  | The name of the site on Netlify. |
| `TOTA_NETLIFY_TOKEN` | Netlify personal access token.   |
