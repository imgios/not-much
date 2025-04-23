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

Once installed, you can configure and customise the theme as you wish - read the [configuration.md](https://github.com/imgios/not-much/blob/main/configuration.md) for more details.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Built With

* [Hugo](https://gohugo.io/) - The static site generator framework
* [Bootstrap](https://getbootstrap.com/) - Free and open-source CSS library
* [Literata](https://fonts.google.com/specimen/Literata) - Used as main theme font
* [RedHat Mono](https://fonts.google.com/specimen/Red+Hat+Mono) - Used as theme code-related font

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contributing

Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please discuss and propose it with the owner. You can also simply open an issue with the tag "enhancement".

Please read [CONTRIBUTING.md](https://github.com/imgios/not-much/blob/main/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to this project.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/imgios/not-much/tags). 

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

<p align="right">(<a href="#readme-top">back to top</a>)</p>