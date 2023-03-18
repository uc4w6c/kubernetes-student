# kindを使ってサービスの作成まで行う

参考: https://qiita.com/tomoyafujita/items/5a3c06705f62c5732bc5
コンテキスト名: kind-service


## 各種コマンド

### クラスタの起動
$ kind create cluster --name kind-service --config=multi-node.yaml

### deployment/serviceの起動
$ kubectl apply -f app-nginx.yaml

### 接続確認
http://localhost:30070/

### クラスタの削除
$ kind delete cluster --name kind-service
