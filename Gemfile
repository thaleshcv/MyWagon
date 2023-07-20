# By default, Wagon 3 doesn't need `bundle exec` to be executed.
# However, if down the road, you want to run a specific version of Wagon or try a new version
# without overriding the global Wagon binary, please use this Gemfile.

source 'https://rubygems.org'

gem 'locomotivecms_wagon', '~> 3.1.1'

group :development do
  # Mac OS X
  gem 'rb-fsevent', '~> 0.10.0', require: 'rb-fsevent' if RUBY_PLATFORM.include?('darwin')

  # Unix
  gem 'therubyracer', require: 'v8', platforms: :ruby unless RUBY_PLATFORM.include?('darwin')

  gem 'rb-inotify', '~> 0.10.0', require: 'rb-inotify' if RUBY_PLATFORM.include?('linux')

  # Windows
  gem 'wdm', '~> 0.1.1', require: 'wdm' if RUBY_PLATFORM =~ /mswin|mingw/i
end
