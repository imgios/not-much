<a id="readme-top"></a>

# not much

<img src="https://raw.githubusercontent.com/imgios/not-much/main/images/tn.png" />

`not-much` is a minimal Hugo theme that I use for my personal website. It doesn't have any fancy shortcode or useless feature.

**It's basic, simple and minimal.**

> 🧪 Demo: https://imgios.github.io/not-much/

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Prerequisites

- Git
- Hugo

### Installing

Clone this repository in your machine:

```shell
$ git clone https://github.com/imgios/not-much.git
```

Change the workdir to `not-much/exampleSite` and start the Hugo server:

```shell
$ cd not-much/exampleSite
$ hugo server -D
hugo server -D
Watching for changes in \not-much\{archetypes,assets,exampleSite,i18n,layouts,static}
Watching for config changes in \not-much\exampleSite\config.toml
Start building sites …
...
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```

Now you are ready to update the theme and see the changes live @ [localhost](http://localhost:1313/).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Deployment

The theme can be installed in two different ways:

1. By adding `not-much` as submodule in your Hugo website repository

```shell
$ cd your-hugo-website
$ git submodule add https://github.com/imgios/not-much.git themes/not-much
```

2. By adding the `not-much` theme dir in `/your-hugo-website/themes/*`

The first option is quite limited as you won't be able to edit the templates if you wanted to. The second option, on the other hand, gives you the entire structure of the theme and allows you to customise it as you wish.

Once done, update (or add) the `theme` parameter in your website configuration file to `theme = not-much`.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Configuration

You can update the website index, menu and copyright directly in your Hugo site `config.toml`.

A reference can be found in [`exampleSite/config.toml`](https://github.com/imgios/not-much/blob/main/exampleSite/config.toml)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

#### Homepage

You can update the homepage by creating the index in `your-hugo-wesbite/content/_index.md` with the following structure:

```yaml
---
lead: "Basic, simple and minimal Hugo theme"
---

This is a demo of the `not-much` theme, built with Hugo, and is intended to be trouble-free. Explore it to see what `not-much` has to offer.
```

Using the page content for the description gives you the flexibility to extend the description by adding inline code, links, lists and more. The use of headings is not really intended there, but feel free to do so if you like.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

#### Menu items and custom links

The main menu can be customised as you prefer to add site-related locations (e.g., your blog location) or your social links:

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

#### Color Palette

This theme lets you select both the theme style and color palette to use in your Hugo website. The default is a dark black and red-ish, but new palettes can be easily added.

Available Color Palettes:
- Default
- Catpuccin
- Dracula

Use the `theme` site param to specify the theme style and `palette` site param to specify the palette name to use. If those param are not specified, the theme will load the default automatically.

```toml
[params]
theme = "dark"
palette = "default"
```

| Param | Allowed values |
|-------|----------------|
| theme | `light, dark, auto` |
| palette | `catpuccin,dracula,default,custom-palette-name` <br/><sub> where `custom-palette-name` is available as `assets/css/palette/custom-palette-name.css` </sub> |

New palettes can be stored under `assets/css/palette`.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

#### Copyright

Write your custom copyright notice in the footer by updating the `copyright` field:

```toml
copyright = "© {year}"
```

The theme notice `// powered by hugo and imgios/not-much` can be enabled (or disabled) by setting the `showThemeNotice` boolean parameter:

```toml
showThemeNotice = true # or false
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

#### Math rendering with KaTeX

You can enable the math rendering by adding `math: true` in the page metadata.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

#### Posts Summary in the Posts list

You can enable the posts summary rendering in the Posts list by configuring the `showPostsSummary` parameter:

```toml
showPostsSummary = true
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

#### Table of Contents

You can display the Table of Contents in the post by configuring the `toc` parameter in the header:

```markdown
---
...
toc: true
---
```

The Table of Contents is not displayed by default.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Built With

* [Hugo](https://gohugo.io/) - The static site generator framework
* [Bootstrap](https://getbootstrap.com/) - Free and open-source CSS library
* [Literata](https://fonts.google.com/specimen/Literata) - Used as main theme font
* [RedHat Mono](https://fonts.google.com/specimen/Red+Hat+Mono) - Used as theme code-related font

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contributing

<!-- Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us. -->
Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1. [Fork the project](https://github.com/imgios/not-much/fork)
2. Create your Feature Branch (`git checkout -b feat/cool-feature`)
3. Commit your Changes (`git commit -m 'add some cool-feature'`)
4. Push to the Branch (`git push origin feat/cool-feature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/imgios/not-much/tags). 

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
