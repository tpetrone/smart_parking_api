source 'https://rubygems.org'

# Specify the Ruby version for Heroku
ruby '2.3.1'

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '>= 5.0.0.rc1', '< 5.1'

# Use the PostgreSQL earthdistance extension with Active Record.
gem 'activerecord-postgres-earthdistance'

# Build JSON APIs with JBuilder.
gem 'jbuilder', github: 'rails/jbuilder', branch: 'master'
gem 'jbuilder-json_api'

# Use PostgreSQL as the database for Active Record.
gem 'pg', '~> 0.18'

# Use Puma as the app server.
gem 'puma', '~> 3.0'

# Use RestClient to communicate with other services from the platform.
gem 'rest-client'

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]

# Plugin for API versioning.
gem 'versionist'

# Devise authentication
gem 'devise'

# Omniauth SSO
gem 'omniauth'

# Token based user Authentication
gem 'devise_token_auth'

# Use Rack CORS for handling Cross-Origin Resource Sharing (CORS), making
# cross-origin AJAX possible.
gem 'rack-cors', require: 'rack/cors'

group :development, :test do
  gem 'byebug',                     platform: :mri
  gem 'factory_girl_rails'
  gem 'faker'
  gem 'flay',                       require: false
  gem 'flog',                       require: false

  # Use the most recent RSpec gems, since they work better with Rails 5.
  ['rspec-core',
   'rspec-expectations',
   'rspec-mocks',
   'rspec-rails',
   'rspec-support'].each do |lib|
    gem lib, github: "rspec/#{lib}", branch: 'master'
  end

  gem 'rspec-collection_matchers'
  gem 'pry'
  gem 'rubocop',                    require: false
  gem 'simplecov',                  require: false
end

group :development do
  # Better errors handler
  gem 'better_errors', '~> 1.0.1'
  gem 'binding_of_caller', '~> 0.7.2'

  # Help to kill N+1 queries and unused eager loading
  gem 'bullet', require: false

  gem 'listen'
  gem 'overcommit'

  # Code metric tool for Rails projects
  gem 'rails_best_practices'

  # Line-profiler for ruby
  gem 'rblineprof', platform: :mri, require: false

  # Rails Console on the Browser.
  gem 'web-console', '~> 2.0'
end

group :production do
  # Heroku
  gem 'rails_12factor'
end

# More default Rails gems:

# Use ActiveModel has_secure_password
# gem 'bcrypt', '~> 3.1.7'

# Use Capistrano for deployment
# gem 'capistrano-rails', group: :development
