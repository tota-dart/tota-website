---
title: "Assets | Tota"
template: "docs"
public: true
---

# Assets

Assets are any static files that Tota doesn't process. For example, images, CSS stylesheets or JavaScript files.

<br>

## Assets directory

The entire assets directory is copied to the `public` directory when Tota builds your site.

For instance, if you had an image called `party-parrot.gif` stored in your assets directory,
you can reference the file in your pages and templates:

```html
<img src="/assets/party-parrot.gif" alt="dancing parrot" />
```

The assets directory location can be changed in the directory [configuration](/docs/configuration#directory).

```bash
TOTA_ASSETS_DIRECTORY="static"
```
