## 概要

Reactの勉強のためのリポジトリ。


## 環境構築まで

### homebrew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

公式サイトのコマンドをそのまま使う
https://brew.sh/index_ja.html

* 前から入ってたのでパス

brew doctor

XCODEが最新じゃないよ的なWARNINGが出たのでXCODEをAppStoreでX Codeを最新にした（いつも思うけど、なんでライブラリ）

### homebrewとnodebrewとnode
brew install nodebrew
↑XCODEが最新じゃないとここでエラーになる

nodebrew
nodebrew setup

export PATH=$HOME/.nodebrew/current/bin:$PATH
export NODEBREW_ROOT=/usr/local/var/nodebrew
sudo vi ~/.bash_profile
source ~/.bash_profile

nodebrew install-binary latest

nodebrew ls
nodebrew use v9.4.0
node -v
npm -v

### React
npm install -g create-react-app

create-react-app sample
cd sample
npm start

なんかサーバーが起動した