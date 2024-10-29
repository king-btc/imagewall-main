source "https://rubygems.org"

ruby "3.1.2"

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

# Bundle edge Rails instead: gem "rails", github: "rails/rails"
gem "rails", "~> 7.0.4"
# Use postgresql as the database for Active Record
gem "pg", "~> 1.4.4"
# Use Puma as the app server
gem "puma", "~> 6.0.0"
# Use SCSS for stylesheets
gem "sass-rails", "~> 6.0.0"
# Use Uglifier as compressor for JavaScript assets
gem "uglifier", ">= 4.2.0"
# Turbolinks makes navigating your web application faster. Read more: https://github.com/turbolinks/turbolinks
gem "turbolinks", "~> 5.2.1"
# User authentication
gem "devise", "~> 4.8.1"
# This is a temporary fix until Devise pushes changes to allow for the previous line
#gem "devise", :git => "git://github.com/plataformatec/devise.git"
# Make those console db queries look sexy
gem "hirb", "~> 0.7.3"
# Create pretty URLs
gem "friendly_id", "~> 5.4.2"
# Use Acts As List for sorting
gem "acts_as_list", "1.0.4"
# Use Figaro for ENV variables
gem "figaro", "~> 1.2"
# AWS integration
gem "aws-sdk", "~> 3.1"
# Imgix
gem "imgix-rails", "~> 4.2.0"
# Auto prefix our CSS
gem "autoprefixer-rails", "~> 10.4.7.0"
# Use Dalli for memcached
gem "dalli", "~> 3.2.3"
# Use will_paginate for User index
gem "will_paginate", "~> 3.3.1"
# font-awesome
gem "font-awesome-sass", "~> 6.2.0"
# Allow for ES6
gem "sprockets-es6"
# Contact form
gem "mail_form", "~> 1.9.0"
# PDF generator (needs wkhtmltopdf on machine to function)
# Local installation: brew install caskroom/cask/wkhtmltopdf
gem "wicked_pdf"
# HTTParty for API requests
gem "httparty", "~> 0.20.0"

gem "tzinfo-data"

gem 'wdm', '>= 0.1.1', :platforms => [:x64_mingw, :mingw, :mswin]

gem "bcrypt", "~> 3.1.18"

gem 'activerecord-session_store'
#added activerecord-session_store on 9/17/2020 in order to address CookieOverflow issue

group :development do
  # Better error pages for debugging
  gem "better_errors"
  # Call "byebug" anywhere in the code to stop execution and get a debugger console
  gem "byebug", platform: :mri
  gem "faker"
  # Access an IRB console on exception pages or by using <%= console %> anywhere in the code.
  gem "web-console"
  gem "listen"
  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem "spring"
  gem "spring-watcher-listen"
  # Allows for REPL use in Rails errors
  gem "binding_of_caller"
end

group :production do
  # Use for static asset serving and logging on Heroku
  gem "rails_12factor", "~> 0.0.3"
  # Installation of wkhtmltopdf for Heroku
  gem 'wkhtmltopdf-heroku'
end
