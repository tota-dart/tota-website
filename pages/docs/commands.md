---
title: "Commands | Tota"
public: true
template: "docs.mustache"
---

# Commands

## init

Creates a new Tota project from the starting [template](https://github.com/tota-dart/tota-starter).

```bash
# Create a site directory
mkdir site && cd site

# Initialize project
tota init
```

Option | Description
--- | ---
`-d`, `--directory` | Specify the directory path (defaults to `"."`)
`-v`, `--verbose` | Enable verbose logging

<br>
<br>

## new

Creates a new page from a title.

```bash
tota new "Hello, world!"
```

Option | Description
--- | ---
`-t`, `--type` | Type of page to create [page, post]
`-f`, `--force` | Force creation of file
`-v`, `--verbose` | Enable verbose logging

<br>
<br>

## build

Generates static files from source pages.

```bash
tota build
```

Option | Description
--- | ---
`-v`, `--verbose` | Enable verbose logging
