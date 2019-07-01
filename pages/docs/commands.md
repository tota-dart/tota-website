---
title: "Commands | Tota"
public: true
template: "docs.mustache"
---

# Commands

Tota is a command-line (CLI) tool available in your terminal. You can invoke its
commands with `tota [command]`.

<br>

## init

Scaffolds a new Tota project in the current directory from the starting
[template](https://github.com/tota-dart/tota-starter).

```bash
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

<br>
<br>

## Deploy

Deploys site to a hosting provider. Currently only deploys to
[Netlify](https://www.netlify.com).

```bash
tota deploy
```

Option | Description
--- | ---
`-p`, `--provider` | Hosting provider (defaults to "netlify")
`-v`, `--verbose` | Enable verbose logging
