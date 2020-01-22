# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:
* ubuntu on windows
参照：https://ja.seo.jxyz.info/ubuntu18-04-on-windows10-easy/
# PowerShellでWSLをインストールする
```
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```
# ubuntu インストール
```
sudo apt-get update
sudo apt-get upgrade -y
```

* Nodejs インストール
```
sudo apt-get install nodejs
sudo apt install -y nodejs npm
sudo npm install n -g
sudo n stable
sudo apt purge -y nodejs npm
exec $SHELL -l
node -v
```
* sqllite インストール
```
sudo apt-get install sqlite3 libsqlite3-dev
```
* Yarn インストール
```
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt update
sudo apt install yarn
yarn --version
```
* Ruby インストール
```
sudo apt-get install ruby
sudo apt-get install rbenv
sudo apt-get install ruby-build
sudo apt-get install ruby-dev
sudo apt-get update
```
* Rail インストール
```
sudo gem install rails
```
* shopify create
```
rails new my_shopify_app
cd my_shopify_app
echo "gem 'shopify_app'" >> Gemfile
bundle install
```
* shopify default Generators
```
rails generate shopify_app
vi .env
SHOPIFY_API_KEY=your api key
SHOPIFY_API_SECRET=your api secret
rails db:migrate
```
* shopify app start
```
bundle exec rails server
http://localhost:3000
```
* shopify  Generator
```
rails generate shopify_app:app_proxy_controller
rails generate shopify_app:add_marketing_activity_extension
rails generate shopify_app:user_model
```
* shopify webhook
```
rails g shopify_app:add_webhook -t carts/update -a https://example.com/webhooks/carts_update
```
* shopify App Tunneling
```
ngrok http 3000
```

* Remote - WSL
install Remote - WSL plugin for vscode
open ubuntu folder in vscode