# Dillon Singh — personal site

Personal technical website built with [Hugo](https://gohugo.io/) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme.

## Requirements

- Hugo extended, version 0.146.0 or later
- Git

## Run locally

```sh
git submodule update --init --recursive
hugo server
```

The site is served at <http://localhost:1313/>.

## Build

```sh
hugo --gc --minify
```

The generated site is written to `public/`.

## Layout

| Path | Contents |
|---|---|
| `config/_default/hugo.toml` | Site title, base URL, copyright |
| `config/_default/menus.toml` | Navigation menu |
| `config/_default/params.toml` | Theme settings and home page profile |
| `content/` | Pages, written in Markdown |
| `assets/images/` | Images used in content pages |
| `assets/css/extended/` | Custom styles |
| `layouts/_shortcodes/img.html` | Image shortcode |
| `static/` | Favicons |
| `themes/PaperMod/` | Theme (git submodule) |

## Add a page

Create a Markdown file in one of the sections under `content/`, for example `content/projects/my-project.md`:

```toml
+++
title = 'My Project'
summary = 'One or two sentences shown on the Projects page.'
weight = 25
tags = ['Python']
+++
```

Pages in Experience, Projects, and Education are ordered by `weight`, lowest first. Blog posts are ordered by `date`.

## Add an image

Put the file in `assets/images/`, then reference it from a content page:

```text
{{</* img src="chart.png" alt="What the image shows" caption="Optional caption" */>}}
```
