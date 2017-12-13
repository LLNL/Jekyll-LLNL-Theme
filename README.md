# LLNL Theme for Jekyll Websites

Author: Ian Lee <lee1001@llnl.gov> and Elsa Gonsiorowski <gonsie@llnl.gov>

## Installation

Add this line to you Jekyll site's `Gemfile`:

```ruby
gem "jekyll-llnl-theme"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
remote_theme: llnl/jekyll-llnl-theme
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jekyll-llnl-theme

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
