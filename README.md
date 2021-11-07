# buildの実行

```docker-compose build```

Gemfile に追記された gem のインストール

# コンテナの起動

```docker-compose up -d```
-dでバックグランド起動

# コンテナ一覧確認方法
```docker ps -a ```

# 不要なイメージやコンテナを削除する方法

コンテナを消す場合は、docker ps -aからコンテナを確認<br>
``` dockr rm コンテナID```
で削除

イメージを消す場合は、<br>
```docker images``` 
からイメージ一覧を確認し、不要なイメージIDを
``` docker rm images ```
で削除

```docker system prune -f ```<br>
停止中のコンテナや未使用ボリュームやイメージやネットワークを全部削除する（未使用オブジェクトを全て削除するため注意）

