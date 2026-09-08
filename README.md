### Thanks for visiting my homepage! :)

This repository pins Ruby 3.4.10 through `.ruby-version`. Use an rbenv-managed
Ruby for the supported project workflow; entering the repository selects the
pinned version automatically. Bundler 2.6.6 is expected.
ImageMagick must also be available because production builds use `jekyll-imagemagick`.

```bash
rbenv install -s 3.4.10
ruby --version
gem install bundler -v 2.6.6
bundle --version
bundle install
```

To build or serve the site from the repository root, run:

```bash
bundle exec jekyll build
# use JEKYLL_ENV=production to preview
JEKYLL_ENV=production bundle exec jekyll serve --host 0.0.0.0 --port 8080
```

To clean up, run:

```bash
bundle exec jekyll clean
rm -rf _site .jekyll-metadata
```

### License

This website is a lightweight customized version of the [al-folio](https://github.com/alshedivat/al-folio) theme (MIT License), based on commit [db2a1d1](https://github.com/alshedivat/al-folio/tree/db2a1d1b1984d00a52b0be1cb74b2b3aefb31ad5), powered by [Jekyll](https://jekyllrb.com/), with improved SASS compatibility and simplified structure.

© 2025-2026 Yixin Chen.
