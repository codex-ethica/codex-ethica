source "https://rubygems.org"

# Use the GitHub Pages gem to ensure compatibility with GitHub Pages build environment
# It includes Jekyll, common plugins (like minima, jekyll-feed, jekyll-seo-tag),
# and sets up Markdown processing (including GFM).
# The version ~> 232 corresponds to what was seen in your GitHub Actions logs.
gem "github-pages", "~> 232", group: :jekyll_plugins

# For local development with Ruby 3+, 'webrick' is needed if the Jekyll
# version used by 'github-pages' doesn't bundle it.
# This conditional addition helps keep local 'bundle exec jekyll serve' working
# without interfering with GitHub Actions.
if Gem.ruby_version >= Gem::Version.new('3.0.0')
  gem "webrick", "~> 1.8"
end

# The 'github-pages' gem typically includes:
# - A compatible version of Jekyll
# - Common plugins like jekyll-feed, jekyll-seo-tag
# - A default theme (minima)
# - kramdown with GFM support
#
# Therefore, explicit declarations like these below might no longer be needed,
# or could even cause conflicts if versions are misaligned with 'github-pages'.
#
# gem "jekyll", "~> 3.9.3" # Handled by github-pages
# gem "kramdown-parser-gfm", "~> 1.1.0" # GFM support is included with kramdown in github-pages
# gem "minima", "~> 2.5" # Usually included/compatible
# group :jekyll_plugins do
#   gem "jekyll-feed", "~> 0.12" # Usually included
#   gem "jekyll-seo-tag", "~> 2.6" # Usually included
# end 