---
title: "Assets | Tota"
template: "docs"
public: true
---

# Assets

Assets are any static files that Tota doesn't need to process. This includes images, CSS and JavaScript files.

<br>

## Directory

The entire `assets` directory is copied to the `public` directory when Tota builds your site.
So, if you had an image called `party-parrot.gif` in your assets directory,
you can easily reference the file in your pages and templates:

```html
<img src="/assets/party-parrot.gif" alt="dancing parrot" />
```

The assets directory location can be changed in the directory [configuration](/docs/configuration#directory).

```bash
TOTA_ASSETS_DIRECTORY="static"
```

<hr />

## Related

- [Pages](/docs/pages)
- [Templates](/docs/templates)
- [Deployment](/docs/deployment)
