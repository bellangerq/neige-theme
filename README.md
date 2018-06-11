# neige-theme

## To do

- [x] Create `/about` page
- [x] Create `/contact` page
- [x] Add scrolling header indicator
- [x] Implement pagination (x posts by page, x being a data variable)
- [x] Put all data in `_config.yml` file
- [x] Set branch master as default branch for GitHub pages
- [ ] Add syntax highlighting
- [ ] Add Google analytics config
- [x] Add lang attribute to HTML and in config
- [x] Add `rel=noopener` to external links

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
