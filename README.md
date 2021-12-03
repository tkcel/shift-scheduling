# Pulp を用いてシフトスケジューリング問題を解く

## 環境構築

- Docker で Jupyter 環境を構築する
  ```
  $ docker-compose up -d
  ```
- http://localhost:8888/ にアクセスして Jupyter 環境に入る
- コンテナ環境に入る
  ```
  $ docker-compose exec notebook bash
  ```
- 必要な python モジュールをインストールする

  ```
  (notebook)$ pip install <package name>
  ```

  > qiita_sample.ipynb を動かすことを考えると
  >
  > - PuLP
  > - ortoolpy

  > が必要

### Docker コンテナ終了

- コンテナを止めて削除する
  ```
  $ docker stop <containerId> && docker rm <containerId>
  ```
