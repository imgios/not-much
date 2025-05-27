<a id="readme-top"></a><h1>Theme Configuration</h1>

Most of the features and configurations are done directly in the Hugo `config.toml`.

A reference can be found in [`exampleSite/config.toml`](https://github.com/imgios/not-much/blob/main/exampleSite/config.toml)

### Table of Contents

- [Homepage](#homepage)
- [Menu items and custom links](#menu-items-and-custom-links)
- [Color Palette](#color-palette)
- [Copyright](#copyright)
- [Math rendering with KaTeX](#math-rendering-with-katex)
- [Posts Summary in the Posts list](#posts-summary-in-the-posts-list)
- [Table of Contents](#table-of-contents)
- [Giscus Comments](#giscus-comments)

## Homepage

You can update the homepage by creating the index in `/content/_index.md` with the following structure:

<kbd>/content/_index.md</kbd>
```yaml
---
lead: "Basic, simple and minimal Hugo theme"
---

This is a demo of the `not-much` theme, built with Hugo, and is intended to be trouble-free. Explore it to see what `not-much` has to offer.
```

Using the page content for the description gives you the flexibility to extend the description by adding inline code, links, lists and more. The use of headings is not really intended there, but feel free to do so if you like.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Menu items and custom links

The main menu can be customised as you prefer to add site-related locations (e.g., your blog location) or your social links:

<kbd>config.toml</kbd>
```toml
# Controls the navigation
[[menu.main]]
  identifier = "about"
  name = "about"
  title = "About"
  url = "/"

[[menu.main]]
  identifier = "posts"
  name = "posts"
  title = "Posts"
  url = "/posts"

[[menu.main]]
  identifier = "github"
  name = "github"
  title = "GitHub"
  url = "https://github.com/imgios"
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Color Palette

This theme lets you select both the theme style and color palette to use in your Hugo website. The default is a dark black and red-ish, but new palettes can be easily added.

Available Color Palettes:
- Default
- Catpuccin
- Dracula

Use the `theme` site param to specify the theme style and `palette` site param to specify the palette name to use. If those param are not specified, the theme will load the default automatically.

<kbd>config.toml</kbd>
```toml
[params]
theme = "dark"
palette = "default"
```

| Param | Allowed values |
|-------|----------------|
| theme | `light, dark, auto` |
| palette | <ul><li>catpuccin</li><li>dracula</li><li>default</li><li>eink</li><li>solarized</li><li>custom-palette-name<br/><sub>where `custom-palette-name` is available as `assets/css/palette/custom-palette-name.css`</sub></li> |

New palettes can be stored under `assets/css/palette`.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Copyright

Write your custom copyright notice in the footer by updating the `copyright` field:

<kbd>config.toml</kbd>
```toml
copyright = "© {year}"
```

The theme notice `// powered by hugo and imgios/not-much` can be enabled (or disabled) by setting the `showThemeNotice` boolean parameter:

<kbd>config.toml</kbd>
```toml
showThemeNotice = true # or false
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Math rendering with KaTeX

You can enable the math rendering by adding `math: true` in the page metadata.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Posts Summary in the Posts list

You can enable the posts summary rendering in the Posts list by configuring the `showPostsSummary` parameter:

<kbd>config.toml</kbd>
```toml
showPostsSummary = true
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Table of Contents

You can display the Table of Contents in the post by configuring the `toc` parameter in the header:

<kbd>/content/posts/example-post.md</kbd>
```markdown
---
...
toc: true
---
```

The Table of Contents is not displayed by default.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Giscus Comments

This theme integrate [Giscus](https://giscus.app/) as comment system, which relies on GitHub Dicussions.

Giscus integration requires the following parameters in site configuration:

<kbd>config.toml</kbd>
```toml
[params.giscus]
repository = "username/repository"
repositoryId = "repositoryId"
categoryName = "categoryName"
categoryId = "categoryId"
mapping = "pathname"
theme = "preferred_color_scheme"
language = "en"
lazyLoading = true
```

Both `repositoryId` and `categoryId` can be fetched from Giscus website.

Once configured, you can enable comments by using the `comments` parameter in the header:

<kbd>/content/posts/post-with-comments.md</kbd>
```markdown
---
...
comments: true
---
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>
