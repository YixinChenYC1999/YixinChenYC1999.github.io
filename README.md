### Thanks for visiting my homepage! :)

To test this page locally, on a Ubuntu machine with zsh, at the homefolder path, run:

```bash
sudo apt install ruby-full build-essential zlib1g-dev
ruby -v
echo '# Install Ruby Gems to ~/gems' >> ~/.zshrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.zshrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
gem install bundler jekyll
jekyll -v
bundle -v
```

Then move to the repo folder, run:

```bash
bundle install
bundle update
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