### Thanks for visiting my homepage! :)

[![Deploy site](https://github.com/YixinChen6/YixinChen6.github.io/actions/workflows/deploy.yml/badge.svg?branch=main)](https://github.com/YixinChen6/YixinChen6.github.io/actions/workflows/deploy.yml) [![Check for broken links on site](https://github.com/YixinChen6/YixinChen6.github.io/actions/workflows/broken-links-site.yml/badge.svg?branch=main)](https://github.com/YixinChen6/YixinChen6.github.io/actions/workflows/broken-links-site.yml) [![CodeQL Advanced](https://github.com/YixinChen6/YixinChen6.github.io/actions/workflows/codeql.yml/badge.svg?branch=main)](https://github.com/YixinChen6/YixinChen6.github.io/actions/workflows/codeql.yml) 
[![pages-build-deployment](https://github.com/YixinChen6/YixinChen6.github.io/actions/workflows/pages/pages-build-deployment/badge.svg?branch=gh-pages)](https://github.com/YixinChen6/YixinChen6.github.io/actions/workflows/pages/pages-build-deployment) [![Check for broken links](https://github.com/YixinChen6/YixinChen6.github.io/actions/workflows/broken-links.yml/badge.svg?branch=main)](https://github.com/YixinChen6/YixinChen6.github.io/actions/workflows/broken-links.yml)

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
bundle exec jekyll build
bundle exec jekyll serve --host 0.0.0.0 --port 8080
```

To clean up, run:

```bash
bundle exec jekyll clean
rm -rf _site .jekyll-metadata
```