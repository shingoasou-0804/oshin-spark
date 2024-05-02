# oshin-spark
## Sparkおよび数理最適化によるプログラムの概念実証

## 必要環境

- docker version 20.10.x 以上

## セットアップ・実行方法

```console
# build
$ docker compose build --no-cache

# boost
$ docker compose up

# fix library version
$ docker compose exec jupyterlab pip freeze > requirements.lock
```

## 注意点
Appleシリコン搭載のMacを使用している場合、Rosseta2を有効にした状態にする。
現時点ではPython-MIPパッケージにソルバーであるCBCがバンドルされていないためである。
