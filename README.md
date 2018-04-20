# LLNL Theme for Jekyll Websites

Author: Ian Lee <lee1001@llnl.gov> and Elsa Gonsiorowski <gonsie@llnl.gov>

## Installation

This gem can be used in two ways: either as a gem-based theme or through GitHub pages remote theme support (details [here](https://github.com/blog/2464-use-any-theme-with-github-pages)).

### Gem-Base Theme

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-llnl-theme"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-llnl-theme
```

And then execute:

```shell
$ bundle
```

Or install it yourself as:

```shell
$ gem install jekyll-llnl-theme
```

### GitHub Pages Remote Theme

This is a recent addition to GitHub pages and is simple to use.
Add this line to your site's `Gemfile`:

``` ruby
gem "github-pages", group :jekyll_plugins
```

And add this line to your site's `_config.yml`:

``` yaml
remote_theme: LLNL/Jekyll-LLNL-Theme
```

It is unclear if the remote theme is suitable for local development, but it will work on deployed sites.

## Usage

This theme supports multiple page websites.
Any page which is located at `/`, such as `/about.md`, will be added to the navigation bar at the top.
Each page should include the following YAML front matter:

```yaml
---
layout: default
title: Title of the Page
---
```

Currently, there is only the `default` layout.

### Adding a Blog

In true Jekyll fashion, a blog can be created by adding a `_posts/` directory.
See the [Jekyll Documentation](https://jekyllrb.com/docs/posts/) for details on formatting blog entries.

The following code is an example of how to create a list of blog entries:

```html
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
```

## Development

### With Ruby Gems

Assuming working on OS X, tested on OS X 10.11.2. `gem` (Ruby package manager)
was preinstalled, so just working from there:

```shell
# Install the dependencies:
$ gem install jekyll

# Build and serve the website
$ jekyll serve --baseurl=''

# Browse to (by default) `localhost:4000` in a web browser
$ open localhost:4000
```

For more information, check out the full documentation at: http://jekyllrb.com/

### With Bundler

Using [Bundler](https://bundler.io):

```shell
# Install the dependencies
$ bundle Install

# Build and serve the website
$ bundle exec jekyll serve --baseurl=''

# Browse to (by default) `localhost:4000` in a web browser
$ open localhost:4000
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/llnl/jekyll-llnl-theme.
This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [LLNL Contributing Guide](https://github.com/LLNL/open-source-guidelines/blob/master/CONTRIBUTING.md) code of conduct.

## Release

This Jekyll theme is released under the MIT License. For more details see the
LICENSE File.

LLNL-CODE-705597
LLNL-WEB-680594
