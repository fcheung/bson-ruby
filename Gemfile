source 'https://rubygems.org'

gem 'json', :platforms => [ :ruby_18, :jruby ]
gem 'rake'

group :development, :test do
  gem 'rspec'
  gem 'rake-compiler'

  if ENV['CI']
    gem 'coveralls', :require => false
  else
    gem 'ruby-prof', :platforms => :mri

    gem 'pry'
    gem 'guard-rspec', :platform => [ :ruby_19, :ruby_20 ]
    gem 'rb-inotify', :require => false # Linux
    gem 'rb-fsevent', :require => false # OS X
    gem 'rb-fchange', :require => false # Windows
    gem 'terminal-notifier-guard'
  end
end
