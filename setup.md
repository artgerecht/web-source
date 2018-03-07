PATH="$PATH:$(ruby -e 'print Gem.user_dir')/bin"

bundle install

bundle exec rake preview

bundle exec rake deploy
