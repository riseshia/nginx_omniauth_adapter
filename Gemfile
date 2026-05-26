source 'https://rubygems.org'

# Specify your gem's dependencies in nginx_omniauth_adapter.gemspec
gemspec

gem 'omniauth-github'
gem 'omniauth-google-oauth2', '>= 0.3.1'
gem 'unicorn'

# Ruby 3.2 stays on legacy stack (sinatra 2 / rack 2);
# Ruby 3.3+ moves to modern stack (sinatra 4 / rack 3 + rackup/webrick).
if Gem::Version.new(RUBY_VERSION) >= Gem::Version.new('3.3')
  gem 'rackup'
  gem 'webrick'
else
  gem 'sinatra', '~> 2.2'
  gem 'rack', '~> 2.2'
  gem 'mechanize', '~> 2.0'
end
