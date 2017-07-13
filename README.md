# LLNL Theme for Jekyll Websites

Author: Ian Lee <lee1001@llnl.gov> and Elsa Gonsiorowski <gonsie@llnl.gov>

## Installation

Add this line to you Jekyll site's `Gemfile`:

```ruby
gem "jekyll-llnl-theme"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-llnl-theme
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jekyll-llnl-theme

## Development

### With Ruby Gems

Assuming working on OS X, tested on OS X 10.11.2. `gem` (Ruby package manager)
was preinstalled, so just working from there:

    # Install the dependencies:
    $ gem install jekyll

    # Build and serve the website
    $ jekyll serve --baseurl=''

    # Browse to (by default) `localhost:4000` in a web browser
    $ open localhost:4000

For more information, check out the full documentation at: http://jekyllrb.com/

### With Bundler

Using [Bundler](https://bundler.io):

    # Install the dependencies
    $ bundle Install

    # Build and serve the website
    $ bundle exec jekyll serve --baseurl=''

    # Browse to (by default) `localhost:4000` in a web browser
    $ open localhost:4000

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/llnl/jekyll-llnl-theme.
This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [LLNL Contributing Guide](https://github.com/LLNL/open-source-guidelines/blob/master/CONTRIBUTING.md) code of conduct.

## Release

This Jekyll theme is released under the MIT License. For more details see the
LICENSE File.

LLNL-WEB-680594
