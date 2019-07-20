---
title: "Posts | Tota"
template: "docs"
public: true
---

# Posts

Blogging is a popular use-case for static-site generators, and Tota makes it easy to create one.

Posts are pages that contain additional information that allow Tota to create blog-specific features like archive and tag pages. Since all posts are pages (but not all pages are posts), everything that applies to [pages](/docs/pages) also applies to posts.

<br>

# Posts directory

Posts are written in Markdown (`.md`) format and are stored in a separate top-level posts directory. Tota will convert these files to HTML and save them in the `public` directory when your site is built.

However, unlike pages, posts will be stored in a nested directory inside the public directory. The name of this directory is the same as the posts directory, which can be changed in the [configuration](/docs/configuration#directory) settings.

Since this sub-directory will be reflected in the final URL, you may wish to rename your posts directory:

```bash
TOTA_POSTS_DIR="blog"
```

This will create a URL structure of `https://www.example.com/blog/hello-world`.

<br>

# Create a post

Create a new post by running the [new command](/docs/commands/#new). This will create a new Markdown file in the posts directory.

```bash
tota new --type post "Talkative Parrot for Sale"
```

This will create the file `posts/talkative-parrot-for-sale.md`. Alternatively, you can manually create files in the posts directory.

<br>

## See also

- [Pages](/docs/pages)
- [Front matter](/docs/front-matter)
- [Templates](/docs/templates)
