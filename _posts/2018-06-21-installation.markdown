---
title: Installation
date: 2018-06-21 12:39:00 Z
description: 'Steps to install Neige to your existing Jekyll website. You can choose
  between two ways: as a standard Jekyll theme or thanks to the GitHub pages integration.'
author: quentin
---

There are two ways to install this theme:

* As a standard Jekyll theme.

* As a remote theme with GitHub pages.

## As a Jekyll theme

1. Add `gem "neige-theme"` to the Gemfile.

2. Run `bundle install`.

3. Add `theme: neige-theme` to the `_config.yaml` file.

4. Run `bundle exec jekyll serve` to view the site in `localhost:3000`.

5. Configure the site's data (see the [Configuration documentation](/2018/06/21/configuration)).

## With GitHub pages

1. Add `gem "github-pages", group: :jekyll_plugins` to the Gemfile.

2. Run `bundle install`.

3. Add `remote_theme: "bellangerq/neige-theme"` in the `_config.yaml` (be sure to remove every other `theme` or `remote_theme` entries).

4. Run `bundle exec jekyll serve` to view the site in `localhost:3000`.

5. Configure the site's data (see the [Configuration documentation](/2018/06/21/configuration)).

> Note: once installed, make sure that pages with pagination enabled are HTML (`.html`) files. As mentioned in the Jekyll documentation, the **jekyll-paginate** plugin doesn't work with Markdown (`.md`) files.

For more information, see the \[GitHub README\](https://github.com/bellangerq/neige-theme) file.