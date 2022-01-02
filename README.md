# Node + React の開発環境

開発したもの：https://github.com/spadr/react-resas-spa

### 動作確認のための手順

```
#このリポジトリをGit cloneする
$ git clone https://github.com/spadr/react-develop.git

#cdを移動
$ cd react-develop

#動かしたいReactのリポジトリをGit cloneする
$ git clone https://github.com/spadr/react-resas-spa.git app

#.env.exampleを.envにリネーム
$ mv .env.example .env

#.envにRESASで取得した自分のAPI_KEYを記入する
$ nano .env
$ vim .env

#イメージをビルドし、コンテナを起動
$ docker-compose up -d --build

#ログを確認
$ docker-compose logs -f node

#必要に応じてコンテナのターミナルを叩く
$ docker-compose exec node /bin/ash

#コンテナを終了
$ docker-compose down

```
