# The Plain

_The Plain_ is a minimalist Jekyll theme, designed to focus on writing that really matters to you and your audience.
Everything else is just a distraction.
Nothing more other than useful and understandable information sharing.
This theme is best suited for a personal blog type, but not limited to that.

P/S: This theme is originally inspired by [Leonard Lamprecht's _leo_ theme](https://github.com/leo/leo.github.io), thanks!

[**Live Demo**](http://heiswayi.github.io/the-plain/)

### Screenshot

![The Plain Screenshot](http://i.imgur.com/8ZXhjfV.png)

### Philosophy

> Minimalism is a masterpiece of tranquility. -- Heiswayi Nrird

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

Therefore, you may not use the 'remote\_theme:' setting instead of 'theme:',
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

[MIT](LICENSE.md)

### Credits

Many thanks to this themes [contributors](https://github.com/heiswayi/the-plain/graphs/contributors)
that help fixing bugs or enhancing source code.

