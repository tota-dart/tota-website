---
title: "Posts | Tota"
public: false
template: "docs.mustache"
---

# Posts

Tota is **blog-aware**, and gives special treatment to pages intended to be blog
posts. Similar to pages, Markdown files will be processed into HTML and saved
in the public directory, but under a nested `posts/` directory. 

You can specify the name of the nested directory by changing the source `posts`
directory name in settings:

```bash
TOTA_POSTS_DIRECTORY="articles"
```
Tota re-uses the source `posts` directory name, so you can configure the end
directory by conf

The default template for blog is 'templates/$NAME.mustache', where $NAME equals the name of the posts directory in configuration settings.
