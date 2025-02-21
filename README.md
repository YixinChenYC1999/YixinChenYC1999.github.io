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
bundle exec jekyll build
bundle exec jekyll serve --host 0.0.0.0 --port 8080
```

To clean up, run:

```bash
bundle exec jekyll clean
rm -rf _site .jekyll-metadata
```