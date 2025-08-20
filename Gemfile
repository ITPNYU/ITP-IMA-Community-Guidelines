source "https://rubygems.org"

gem "jekyll", "~> 4.3"
gem "webrick"

# Force Bundler to use the EXACT pre-compiled versions from Ruby 3.3.
# This removes all ambiguity and is the definitive fix.
gem "bigdecimal", "3.1.5"
gem "json", "2.7.1"

# Explicitly added gems no longer bundled by default in modern Ruby.
gem "csv"
gem "base64"

gem "minima"

group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-seo-tag"
end

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]