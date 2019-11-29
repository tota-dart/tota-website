---
title: "Templates | Tota"
template: "docs"
public: true
---

# Templates

Templates defines the presentation of your website by setting the HTML structure. Tota uses [Mustache](http://mustache.github.io/) as its templating language.

<br />

## Directory

Templates are written in Mustache (`.mustache`) format and stored in the [templates directory](/docs/configuration#directory). Tota will insert the page content into the templates when generating the HTML files.

<br />

## Lookup order

Tota follows a simple strategy for resolving which template to use, starting from the most specific and following a series of fallback templates.

An explicit declaration in the [front matter](/docs/front-matter) takes all precedence:

```yaml
---
title: "Parrots & Cockatoos"
template: "birds.mustache"
---

```

If no template can be found, Tota will fallback to either `pages.mustache` or `posts.mustache`, depending on the type of page being generated. Changing the pages/posts directory configuration will have an effect on this lookup.

Finally, Tota will try to resolve `base.mustache` before throwing an error.

<br />

## Partials

Partials are small snippets of reusable code, useful to share components between templates. Common examples include headers, footers, navbars and sidebars.

Partials are mustache templates stored in a `_partials` directory within the templates directory. Render partials inside other templates using the following syntax (omitting the file extension).

```html
{{> sidebar }}
```
