# README

## 初回起動時

1. サービスのビルド
```
docker-compose build
```
2. dbを作成
```
docker-compose run app rails db:create
```
3. テーブルデータ読み込み
```
docker-compose run app rails db:migrate
```
4. 授業データ読み込み
```
docker-compose run app rails db:seed
```
5. サービスの起動
```
docker-compose up
```

## Mysqlのコンソールを起動
```
docker-compose run app rails dbconsole
```

## railsのコンソールを起動
```
docker-compose run app rails console
```

<!-- ## error対応
* docker-compose up でerrorが出た時
 * tmp/pids/server.pid を消してみてください
  -->