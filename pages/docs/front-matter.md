---
title: "Front matter | Tota"
template: "docs"
public: true
---

# Front-matter

Front-matter is a block of YAML at the beginning of a page file, ahead of any Markdown content. The front-matter contains metadata about the page itself:

```yaml
---
title: "Parrots and Cockatoos"
template: "birds.mustache"
date: "2019-08-14 22:33:44"
public: true
---
```

<br>

## Metadata

The following table lists the pre-defined metadata that you can set in the front-matter of your page, or post.

Key | Default | Description
--- | --- | ---
`title` | [`TOTA_TITLE`](http://localhost:5000/docs/configuration#site) | The title of the page.
`description` | [`TOTA_DESCRIPTION`](http://localhost:5000/docs/configuration#site) | A short description of the page.
`public` | `false` | [Boolean] Only public files will be generated, the rest will be skipped.
`template` | `"base.mustache"` | The mustache HTML template to use.
`date` | Current date | A date in `YYYY-MM-DD HH:MM:SS` format. The hours, minutes, and seconds are optional.
`tags` | - | A [YAML list](https://en.wikipedia.org/wiki/YAML#Basic_components) of tags.
