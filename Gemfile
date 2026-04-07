source 'https://rubygems.org'

gem 'jekyll'

gem 'sass-embedded', '~> 1.95'

# Core plugins that directly affect site building
group :jekyll_plugins do
    gem 'jekyll-email-protect'
    gem 'jekyll-imagemagick'
    gem 'jekyll-scholar'
    gem 'jekyll-sitemap'
    gem 'jekyll-terser', :git => "https://github.com/RobertoJBeltran/jekyll-terser.git"

    gem 'classifier-reborn'  # used for content categorization during the build
end

# Gems for development or external data fetching (outside :jekyll_plugins)
group :other_plugins do
    gem 'css_parser'
    gem 'feedjira'
    gem 'httparty'
    gem 'observer'       # used by jekyll-scholar
    gem 'ostruct'        # used by jekyll-twitter-plugin
end
