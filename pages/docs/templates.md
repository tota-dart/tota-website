---
title: "Templates | Tota"
template: "docs"
public: true
---

# Templates

Templates define the HTML structure of your website and allow you to change its presentation and style. Tota uses the [Mustache](http://mustache.github.io/) templating language, which works by substituting variable placeholders for real data.

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>{{title}}</title>
  </head>
  <body>
    <h1>Hello, {{name}}!</h1>
  </body>
</html>
```

<br />

## Directory

Templates are written in Mustache (`.mustache`) format and stored in the [templates directory](/docs/configuration#directory). Tota will insert
the page content into the templates when generating the HTML files.

<br />

## Lookup order

Tota follows a pre-defined strategy to resolve which template to use, starting from the most specific and following a series of fallback
templates.

An explicit template declaration in the [front
matter](/docs/front-matter) takes the highest order of precedence.

```yaml
---
title: "Parrots and Cockatoos"
template: "birds.mustache"
---

```

If no template can be found, Tota will fallback to either `pages.mustache` or `posts.mustache`, depending on the type of page being generated. Note that changing the pages/posts directory names in configuration will have an effect on this lookup.

Finally, Tota will try to resolve `base.mustache` before throwing an error.

<br />

## Partials

Partials are small snippets of reusable code, useful to share components between templates. Common examples include headers, footers, navbars and sidebars. They are stored in a `_partials` directory within the templates directory.

You can import partials inside other templates using the following syntax (omitting the `.mustache` file extension).

```html
{{> sidebar }}
```
