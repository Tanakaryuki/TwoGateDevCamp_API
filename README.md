# 開発方法

## コンテナビルド

`docker build --tag fastapi-demo .`

## コンテナの起動

`docker run  --publish 3100:80 fastapi-demo uvicorn main:app --host 0.0.0.0 --port 80 --reload`

## コンテナの確認

`docker ps`

## コンテナの停止

`docker stop {CONTAINER ID}`

## コンテナの削除

`docker rm {CONTAINER ID}`

## ngrok の起動

`ngrok http 3100`

## コンテナのデプロイ

`aer run  --publish 3100:80 fastapi-d
z acr build   --resource-group web-app-simple-rg   --registry twogate   --image webappsimple:latest .`
