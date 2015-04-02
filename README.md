# cybertrap
[cybertrap.com](https://cybertrap.com) website.

The CMS is built with [middleman](https://middlemanapp.com/). Middleman creates static websites out of the data in the source directory.

middleman requires [Ruby](https://www.ruby-lang.org/en/) and [rubygems](https://rubygems.org/) (is part of the Ruby environment).

To setup the local environment, install [bundler](http://bundler.io/) and install the gems:

```
gem install bundler
bundle
```


## Overview

This template uses [Haml](http://haml.info/) for markup, [Sass](http://sass-lang.com/) & [Autoprefixer](https://github.com/postcss/autoprefixer) for stylesheets, and [CoffeeScript](http://coffeescript.org/) for scripts. It also ships with the handy Middleman extension [middleman-livereload](https://github.com/middleman/middleman-livereload).

Stylesheet and script architecture is designed with the idea of components in mind -- independent, self-contained files designed for a specific purpose.

For stylesheets, these live in the `source/stylesheets/components` directory. For scripts, these live in the `source/javascripts/modules` directory. Modules are components. JavaScript components are called modules simply for the sake of distinguishing what type of component you can refer to.


## Usage

```
# Fire up a local development server
bundle exec middleman server

# Publish a build
bundle exec rake publish
```

## File Structure

```
|_ source/
|  |_ images/
|  |_ javascripts/
|  |  |_ modules/              # Self-contained modules
|  |  |_ vendor/               # Third-party scripts
|  |
|  |_ layouts/
|  |
|  |_ stylesheets/
|     |_ config/               # App-wide style config
|     |_ components/           # Self-contained components
|     |_ vendor/               # Third-party styles
```
