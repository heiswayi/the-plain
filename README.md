# The Plain

> The Plain is a minimalist Jekyll theme, ideally designed for your personal blog use. This Jekyll theme provides a minimum distraction so you can focus on writing that matters to you and your readers. This theme is originally inspired from [Leonard Lamprecht's _leo_ theme](https://github.com/leo/leo.github.io).

[![LICENSE](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE) ![GENERATOR](https://img.shields.io/badge/made_with-jekyll-blue.svg) ![VERSION](https://img.shields.io/badge/current_version-4.0-green.svg) ![TRAVIS-CI](https://travis-ci.org/heiswayi/the-plain.svg?branch=master)

- **Demo:** https://heiswayi.github.io/the-plain/

![SCREENSHOT](https://i.imgur.com/FITKN1H.png)

## Usage

### On an unlimited Jekyll host

> **NOTE** This does NOT work on GitHub, see the next section.

Put this in your *Gemfile*:

	gem 'the-plain'

and run `bundle install` to install the plugin.

Add this to your sites *_config.yml* file:

	theme: the-plain

Then copy some of the settings from this repo's *_config.yml* file to your own, and modify them.

### On GitHub

GitHub - for your user account pages or repository gh-pages - only supports a limited set of themes.

Therefore, you need to use the 'remote\_theme:' setting instead of 'theme:', which is supported by [a 3rd party plugin](https://github.com/benbalter/jekyll-remote-theme).

Put this in your *Gemfile*:

	gem 'jekyll-remote-theme'

and run `bundle install` to install the plugin.

Add the following to your site's *_config.yml* to activate the plugin and to select this theme:

	plugins:
	  - jekyll-remote-theme

	remote_theme: heiswayi/the-plain

This will grab the theme directly from the GitHub repo.

Now copy some of the settings from this repo's *_config.yml* file to your own, and modify them.

## Authors

- [**Heiswayi Nrird**](https://heiswayi.nrird.com)

See also the list of [contributors](https://github.com/heiswayi/the-plain/graphs/contributors) who participated in this project.

## License

[MIT](LICENSE)
