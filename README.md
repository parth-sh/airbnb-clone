1. Installation of rbenv

    1.1. brew install rbenv ruby-build

2. Setting up ruby enviroment

    2.1. rbenv install 3.2.2
    
    2.2. rbenv local 3.2.2

3. Init project
    
    3.1. gem install rails
    
    3.2. brew install postgresql 
    
    3.3. rails new airbnb-clone -T -d postgresql --css tailwind
    
    3.4. cd airbnb-clone/
    
    3.5. brew services start postgresql
    
    3.6. bundle exec rails db:create 
    
    3.7. bundle exec rails s

4. Part1 yt video:

    Defined home route	

    Trimmed body tag
    
    Added favicon
    
    Added Rspec, bundle install, rails generate rspec:install

    Added Devise for user authentication, bundle exec rails generate devise:install
      ```
      Depending on your application's configuration some manual setup may be required:
      
        1. Ensure you have defined default url options in your environments files. Here
          is an example of default_url_options appropriate for a development environment
          in config/environments/development.rb:
      
            config.action_mailer.default_url_options = { host: 'localhost', port: 3000 }
      
          In production, :host should be set to the actual host of your application.
      
          * Required for all applications. *
      
        2. Ensure you have defined root_url to *something* in your config/routes.rb.
          For example:
      
            root to: "home#index"
          
          * Not required for API-only Applications *
      
        3. Ensure you have flash messages in app/views/layouts/application.html.erb.
          For example:
      
            <p class="notice"><%= notice %></p>
            <p class="alert"><%= alert %></p>
      
          * Not required for API-only Applications *
      
        4. You can copy Devise views (for customization) to your app by running:
      
            rails g devise:views
            
          * Not required *
      ```
    Generate devise model, bundle exec rails g devise user

    Migrate database, bundle exec rake db:migrate

    Generate views for devise, bundle exec rails g devise:views

    Added daisyUI cdn stylesheet link

    Making header Navbar by daisy UI components

    Using scss files in stylesheets, Install gem "sassc-rails"

5. Part2 YT video

    Fixed scss pre-compiler error for, config/manifest.js

    Added npm install el-transition, ./bin/importmap pin el-transition
    
    Added closing transtion for header nav menu items
    