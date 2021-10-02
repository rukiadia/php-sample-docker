# CakePHPを動かす手順

```bash
$ docker-compose build 
$ docker-compose up

# PHPコンテナ内へ移動
$ docker exec -it php-sample-docker_php-fpm_1 bash

# CakePHPをインストール
$ composer create-project --prefer-dist cakephp/app:4.* my_app
```

http://localhost でCakePHPの画面が開ける

# 環境
- docker: 20.10.8
- docker-compose 3系
