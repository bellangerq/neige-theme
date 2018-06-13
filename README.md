# Neige

> Neige is a minimalist and lightweight Jekyll blog theme :snowflake:

![Neige theme preview]()

## Table of content

- [Features](#features)
- [Installation](#installation)
- [Configuration](#configuration)
- [How to](#how-to)
  - [Add new post](#add-new-post)
  - [Add new lage](#add-new-page)
  - [Edit error page](#edit-error-page)
  - [Update styles](#update-styles)
- [Development](#development)

## Features

- Made for blogging
- Minimalist
- Fast: no JS
- Accessible
- Easy configuration
- Siteleaf ready
- Meta tags ready
- Works on any browser
- Mobile ready
- Pixel perfect

## Installation

- Gem based
- GH pages

## Configuration

Everythings happens in the `_config.yml` file.

- `title`: set the main title (used for meta tags).

- `description`: set the main description (used for meta tags).

- `favicon`: set the favicon (located at `assets/img/favicon.png`).

- `icon`: set the logo on the header (located at `assets/img/icon.png`).

- `og_image`: set the default Open Graph image (located at `assets/img/og.jpg`).

- `lang`: set the language of your website. Used as `lang` attribute on the `<html>` tag.

- `baseUrl`: set the root URL of your website (example: `https://my-site.com`).

- `twitter`: the main Twitter account of the website (example: `@twitter`).

- `navigation`: set the navigation of your website. Add items with the following properties:

  ```yml
  navigation:
  - name: About
    url: "/about"
    title: About me
    external: false
  - name: Contact
    url: "/contact"
    title: Contact me
    external: false
  ```

  > The `title` property is used as the `title` attribute on the link. Set `external` to "true" if the link should open in a new tab.

- `authors`: Add authors to your blog with the following properties:

  ```yml
  - id: bilbo
    name: Bilbo Baggins
    twitter: "@bilbo"
  ```

  Then you can link a blog post to an author with its `id`.

- `footer`: set custom content for the `<footer>` tag.

- `paginate`: define the number of posts displayed on the page.

- `paginate_path`: define the path of pagination pages (example: `"/blog/page:num/"` would result in `/blog/2/`).

## How to

### Add new post

To create a new blog post, follow these steps:

1. Create a `.md` file in the `_posts` folder (example: `YYYY-MM-DD-post.md`).
2. Add the following properties in the YAML Front Matter:

  ```yml
  ---
  layout: post
  date: YYYY-MM-DD
  title: "Your post title"
  description: "Your post description"
  author: jack
  ---
  ```

  > The `title` and `description` are used on the post but also for the meta tags. The `author` must be a existing author `id` in your `_config.yml` file.

3. Write with blog post content.

### Add new page

To create new static pages, follow these steps:

1. Create a `.md` file at the root of your project (example: `page.md`).
2. Add the following properties in the YAML Front Matter:

  ```yml
  ---
  layout: page
  title: "Your page title"
  description: "Your page description"
  ---
  ```

  > The `title` and `description` are used on the page but also for the meta tags.

3. Write the content of your page.

### Add meta tags

Meta tags for all kind of page (home, page, post and error) are already configured based on the content you're filling in `_config.yml` for the homepage and in the front-matter for the others.

If you wish to modify the behavior of already existing meta tags settings or to add new ones, head over the `head.html` partial in `_includes` folder.

### Edit error page

Simply edit the content of the `404.md` page.

### Update styles

All the `.scss` files are in the `_sass` folder arranged by components (header, pagination, footer...). They are called by the main stylesheet `/assets/css/style.scss`.

Feel free to modify styles the way you want (SASS variables are located in `_sass/vars.scss`).

## To do

- [ ] Add syntax highlighting
- [ ] Add Google analytics config
- Write default posts:
  - [ ] Neige Features
  - [ ] Page elements
  - [ ] Install Neige to your Jekyll website
  - [ ] Make Neige your own
- Write default pages:
  - [ ] About page

## Questions

- Gems: in `.gemspec` or `Gemfile`?
- Difference between GH pages remote theme and classic Jekyll theme
- Versioning configuration (master branch // dev branch)

## Development

Launch local web server with live reloading (port = 4000):

```shell
bundle exec jekyll serve --livereload
```
