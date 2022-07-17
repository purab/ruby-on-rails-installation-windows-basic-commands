install ruby on rails on windows 10

1. go to https://nodejs.org/en/ and download LTS (long time support) nodejs and install it
2. https://classic.yarnpkg.com/en/docs/install#windows-stable - install yarn packages
3. https://www.sqlite.org/download.html -  donwload "64-bit DLL (x64) for SQLite" and "A bundle of command-line tools for managing SQLite database files, including the command-line shell program, the sqldiff.exe program, and the sqlite3_analyzer.exe program."
extract and copy files to "windows/system32 folder". 
Edit environment variables and add sqlite3 there.
4. https://rubyinstaller.org - download and install it on windows
4. open command line and run "gem install sqlite3"
5. open command line and run "gem install rails"
6. Installation is complete. now check versions
ruby --version
sqlite3 --version
node --version
yarn --version
gem --version
rails --version

run ruby file
ruby ./hello.rb

###create new rails project
rails new <projectname>

###start rails server
rails server

###some rails commands
rails server (rails s)
rails console (rails c)
rails generate (rails g)

rails generate controller root

run your database migrations:
rails db:migrate

rails generate controller home index

yarn add bootstrap jquery popper.js

add bootstrap css and js - https://getbootstrap.com/docs/5.2/getting-started/introduction/
in application.html.erb - app/views/layout/application.html.erb

create model

rails g model Post title:string description:text

schema will be found in test/fixtures/posts.yml. following command will execute db migration
rails db:migrate

command to run
-rails console
-Post.connection
-a=Post
-a=Post.new
-a.title="hello"
-a.description="world"
-a.save
-a
-Post.find(1)
-Post.find(1).destroy

use "bundle" command when you are uncomment gemfile line.

-rails g controller sessions
-rails g controller users
-rails g model User email:uniq password:digest
-rails db:migrate