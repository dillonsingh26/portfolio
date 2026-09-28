# Dillon Singh — personal site

Personal technical website built with [Hugo](https://gohugo.io/) and the [Clean White](https://github.com/zhaohuabing/hugo-theme-cleanwhite) theme.

## Requirements

- Hugo extended
- Git

## Run locally

```sh
git submodule update --init --recursive
hugo server
```

The site is served at <http://localhost:1313/>.

## Layout

| Path | Contents |
|---|---|
| `hugo.toml` | Site title, base URL, menu, sidebar, and theme settings |
| `content/post/` | Blog posts, written in Markdown |
| `content/about/` | About page |
| `static/img/` | Header images, avatar, and favicon |
| `assets/images/` | Images placed with the `img` shortcode |
| `layouts/_shortcodes/img.html` | Image shortcode |
| `themes/hugo-theme-cleanwhite/` | Theme (git submodule) |

## Image credits

- `static/img/home-bg-nyc.jpg` — [Midtown Manhattan from Weehawken September 2021 HDR panorama](https://commons.wikimedia.org/wiki/File:Midtown_Manhattan_from_Weehawken_September_2021_HDR_panorama.jpg) by King of Hearts, licensed [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0). Resized from the original.
