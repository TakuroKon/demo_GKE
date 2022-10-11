
# Dockerfile_for_GCR とは

Dockerfile_for_GCR　はGCRへアップロードするサンプルです。
以下のアプリケーションを構成したDockerFileです

- 8080ポートでhollo world を表示するだけ
- golangで書かれたWEBアプリケーション

# 起動方法

- カレントディレクトリをDockerfile_for_GCRフォルダ内にする
- 以下のコマンドでdocker image をビルドする

```
docker build . 
```

- 以下のコマンドでdocker をRUNする

```
docker run -p 8080:8080 {docker ID}
```

- 上記が成功すれば、以下ページにhello world と表示される

http://localhost:8080
