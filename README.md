# README

This README would normally document whatever steps are necessary to get the
application up and running.

# 0. バージョン
- ruby -> 2.7.4
- rails -> 6.1.7
- docker compose -> 3.8
- vue -> 3

# 1. 環境構築
### 1-1. Gitリポジトリをクローン
git clone https://github.com/carbohydratepro/vue.git

cd vue

### 1-2. dockerイメージをbuild
docker-compose build

### 1-3. Dockerを起動
docker-compose up -d

### 1-4. コマンドを実行
docker-compose run web rake db:create

docker-compose run web bundle install

docker-compose run web bundle exec rake app:update:bin

### 1-5. localhost:3000にアクセス
Railsの画面が表示されていれば成功

# 2. 参考サイト
### Railsその他諸々の環境構築
https://prograshi.com/framework/rails/docker-rails6-vue-vuetify/

### vue.jsのインストール
https://universato.hatenablog.com/entry/2021/07/16/025001

# 3. 備考
Rails7系だとWebpackerが使えず、vue.jsの導入が私の技量では厳しかったため、Rails6系で環境を構築している。

