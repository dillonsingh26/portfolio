+++
title = 'Rebuilding This Site with Hugo'
date = 2026-09-28
description = 'How this site is put together: a static site generator, Markdown, and a handful of config files.'
tags = ['Hugo', 'Markdown']
+++

This site is built with [Hugo](https://gohugo.io/), a static site generator written in Go. Hugo takes layout files and content files and generates plain HTML. There is no database and no back-end server.

## How it's organized

Every page is a Markdown file under the `content` directory, and the directory tree is the site structure:

```text
content/
├── about.md
├── resume.md
├── experience/
├── projects/
├── education/
└── blog/
```

Each main section holds one level of pages. Adding a project means adding one Markdown file to `content/projects`.

## Configuration

The configuration is written in TOML and lives under `config/_default`:

- `hugo.toml` — site title, base URL, and copyright
- `menus.toml` — the navigation menu
- `params.toml` — theme settings, including the home page profile

## Theme

The theme is [PaperMod](https://github.com/adityatelange/hugo-PaperMod), added to the repository as a git submodule.

## Images

Images live under `assets/images`. A short Go template pulls an image from that directory, resizes it, and converts it to WebP when the site builds. The chart on the [Chicago Bulls valuation page]({{< relref "/projects/bulls-valuation" >}}) is produced this way.
