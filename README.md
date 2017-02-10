Basic Template for Jekyll formatted for the Laboratory
======================================================

Author: Ian Lee <lee1001@llnl.gov>

## Setup / History

This branch is the upstream branch of the Jekyll LLNL Theme. This template can
be updated by rebasing (or merging) the changes from upstream at:
https://mystash.llnl.gov/projects/LWDS/repos/jekyll-llnl-theme/browse

This uses Jekyll to build static HTML based on Markdown text files.

## Quickstart

Assuming working on OS X, tested on OS X 10.11.2. `gem` (Ruby package manager)
was preinstalled, so just working from there:

    # Install the dependencies:
    $ gem install jekyll
    $ gem install rdiscount

    # Build and serve the website
    $ jekyll serve --baseurl=''

    # Browse to (by default) `localhost:4000` in a web browser
    $ open localhost:4000

For more information, check out the full documentation at: http://jekyllrb.com/

## Quickstart -- Bundler

Using [Bundler](https://bundler.io):

    # Install the dependencies
    $ bundle Install

    # Build and serve the website
    $ bundle exec jekyll serve --baseurl=''

    # Browse to (by default) `localhost:4000` in a web browser
    $ open localhost:4000

## Release

This Jekyll theme is released under the MIT License. For more details see the
LICENSE File.

LLNL-WEB-680594
