コンテナ内にログインします。

\$ docker-compose exec vuesplash_web bash

Laravel プロジェクトを作成します。
コンテナ内

\$ composer create-project --prefer-dist laravel/laravel .

開発用サーバーを立ち上げます。
コンテナ内

\$ php artisan serve --host 0.0.0.0 --port 8081

ホスト側から実行するのであれば、以下のコマンドになります。

\$ docker-compose exec vuesplash_web php artisan serve --host 0.0.0.0 --port 8081

npm コマンドを実行しますが、その場合も artisan コマンドと同様です。
例

$ docker-compose exec vuesplash_web npm install
$ docker-compose exec vuesplash_web npm run watch
