# manurs web site source code

## Offline
https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/

1. Installa ruby and bundler
```
ruby --version # If you dont have ruby, install ruby
gem install bundler
```
2. Create page or clone repo
```
# Create the page with github pages or offline (See github help. Offline require two steps repo+Jekyll)
```
3. Create 'Gemfile'. Content:
```
source 'https://rubygems.org'
gem 'github-pages', group: :jekyll_plugins
```
4. Install dependencies
```
bundle install
apt install ruby2.x-dev # if fails
```
RUN
```
bundle exec jekyll serve
(http://localhost:4000)
```
UPDATE
```
bundle update github-pages
```