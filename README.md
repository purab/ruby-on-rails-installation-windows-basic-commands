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


