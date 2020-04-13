# Memoirs Jekyll Theme
Based on [jekyll-theme-memoirs.git](https://github.com/wowthemesnet/jekyll-theme-memoirs.git) |
[Live Demo](https://wowthemesnet.github.io/jekyll-theme-memoirs/) | [Docs & Download](https://bootstrapstarter.com/bootstrap-templates/jekyll-theme-memoirs/) |
![memoirs](https://bootstrapstarter.com/assets/img/themes/memoirs-jekyll.jpg)


```console
brew install ruby
ruby -v ##(should be >2.40)
export PATH="/usr/local/opt/ruby/bin:$PATH" >> ~/.bash_profile
gem install --user-install bundler jekyll
gem install -n /usr/local/bin jekyll
git clone https://github.com/aliaskov/beseder-life-blog.git
cd jekyll-theme-memoirs/
gem install bundler
bundle install
# edit _config.yml If your site is in root: baseurl: ''.
# Also, change your Google Analytics code,username, authors, Mailchimp list etc.
bundle exec jekyll serve --watch
# Push static site to AWS S3
bundle install s3_website
gem install -n /usr/local/bin s3_website
s3_website cfg create
# Edit s3_website.yml
s3_website cfg apply
s3_website push
```
