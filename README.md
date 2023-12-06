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

