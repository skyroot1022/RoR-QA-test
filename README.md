# What is QARoR?
It's another Questions & Answers platform for Ruby on Rails

# Install on Heroku (heroku.com)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/mateuszdw/qaror)

### Install manually on Heroku

Before installation:

* You need Ruby. Easest way to get RUBY is install RVM (Ruby Version Manager) https://rvm.io/rvm/install
* You also need GIT $ sudo apt-get install git
* To deploy QARoR on Heroku you need Heroku Toolbelt - https://toolbelt.heroku.com/ and confirmed Heroku Account.

Type in console:

        $ bundle install
        $ git init
        $ git add .
        $ git commit -m "init qaror app"
        $ heroku apps:create your-qaror-app-name
        $ git push heroku master
        $ heroku run rake db:migrate
        $ heroku run rake db:seed

Default QARoR installation is adapted to this Heroku Addons:

        $ heroku addons:add mailgun:starter
        $ heroku addons:add memcachier:dev
