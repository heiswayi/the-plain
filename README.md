# The Plain

[![LICENSE](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

The Plain is a minimalist Jekyll theme, ideally designed for personal blog use. This Jekyll theme provides a minimum distraction so you can focus on writing that matters to you and your readers. This theme is originally inspired from [Leonard Lamprecht's _leo_ theme](https://github.com/leo/leo.github.io).

- [**Demo**](https://heiswayi.github.io/the-plain/)

### Screenshot

![The Plain Screenshot](http://i.imgur.com/8ZXhjfV.png)

### How to use

#### on an unlimited jekyll host

**NOTE** This does NOT work on github, see the next section.

Put this in your *Gemfile*:

	gem 'the-plain'

and run `bundle install` to install the plugin.

Add this to your sites *_config.yml* file:

	theme: the-plain

Then copy some of the settings from this repos *_config.yml* file to your own,
and adjust them.

#### on github

GitHub - for your user account pages or repository gh-pages -
only supports a limited set of themes.

Therefore, you need to use the 'remote\_theme:' setting instead of 'theme:',
which is supported by [a 3rd party plugin](https://github.com/benbalter/jekyll-remote-theme).

Put this in your *Gemfile*:

	gem 'jekyll-remote-theme'

and run `bundle install` to install the plugin.

Add the following to your site's *_config.yml* to activate the plugin
and to select this theme:

	plugins:
	  - jekyll-remote-theme

	remote_theme: heiswayi/the-plain

This will grab the theme directly from the github repo.

Now copy some of the settings from this repos *_config.yml* file to your own,
and adjust them.

### License

[MIT](LICENSE)

### Credits

Many thanks to this theme's [contributors](https://github.com/heiswayi/the-plain/graphs/contributors) that help fixing bugs or enhancing source code.