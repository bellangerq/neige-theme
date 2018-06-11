# neige-theme

## Installation

- Gem based
- GH pages

## Customization

- **Logos**: replace the default `icon.png` and `favicon.png` in the `assets/img` folder by your own website's logo and favicon.

- **Open Graph image**: replace the default `og.png` in the `assets/img` folder by your own website's Open Graph image.

- `title`: The main title of your website. Used for meta tags.

- `description`: The main description of your website. Used for meta tags.

- `lang`: the language of your website. Used as `lang` attribute on the `<html>` tag.

- `baseUrl`: the root URL of your website (example: `https://my-site.com`).

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

  > Set `external` to "true" if the link should open in a new tab.

- `authors`: Add authors to your blog with the following properties:

  ```yml
  - id: bilbo
    name: Bilbo Baggins
    twitter: "@bilbo"
  ```

  Then you can link a blog post to an author with its `id`.

- `footer`: set custom text (or HTML) for the `<footer>` tag content.

- `paginate`: define the number of posts displayed on the page.

- `paginate_path`: define the path of pagination pages (example: `"/blog/page:num/"` would result in `/blog/2/`).

## To do

- [ ] Add syntax highlighting
- [ ] Add Google analytics config
- [ ] Complete documentation
- Write fake posts:
  - [ ] Neige Features
  - [ ] Page elements
  - [ ] Install Neige to your Jekyll website
  - [ ] Make Neige your own
- Write fake pages:
  - [ ] About page

## Documentation

- Change pagination settings (number of posts per page, url)
- Add / remove items
- Change icon in header
- Write global info about site
- Change footer content
- Manage authors
- Define page meta data (title, description)
- Change error page content
- Update styles
- Writing post (fill all infos, layout is 'post', add author 'key', date format: '2015-11-17', do not include main title in the content)

## Questions

- Gems: in `.gemspec` or `Gemfile`?
- Difference between GH pages remote theme and classic Jekyll theme
- Versioning configuration (master branch // dev branch)

## Development

Launch local web server with live reloading (port = 4000):

```shell
bundle exec jekyll serve --livereload
```
