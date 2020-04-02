**Upgrading ruby**

brew update && brew upgrade ruby-build
rbenv install 2.6.6
gem install bundler -v 2.1.4
bundle install

**Upgrading node**

nvm install 12.15.0
nvm alias default 12.15.0
nvm use default
