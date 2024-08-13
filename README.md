## 概要
Djangoのサンプルコードです

## 起動方法

1. Visual Studio Codeで開く
- File > Open Folder... エクスプローラからdjango-basical-appを選択

2. ビルドと起動
- TERMINALを開き、以下を実行
docker-compose up --build

4. Docker Containerで開く
左下の[><]アイコン Open a remote windowを選択、Reopen in Container > Main

5.src/sample へ移動
- TERMINALを開き、以下を実行
cd sample

6. ローカルで起動する
- 以下を実行
python manage.py runserver 127.0.0.1:8080

7. 確認
以下へアクセスする
http://127.0.0.1:8080

## トラブルシューティング

### docker daemon is not running

Docker Desktop が起動できていないので起動させましょう

### Ports are not available: address already in use

別のコンテナもしくはローカル上ですでに使っているポートがある可能性があります
<br>
下記記事を参考にしてください
<br>
[コンテナ起動時に Ports are not available: address already in use が出た時の対処法について](https://qiita.com/shun198/items/ab6eca4bbe4d065abb8f)

### Module not found

make build

を実行して Docker image を更新してください
