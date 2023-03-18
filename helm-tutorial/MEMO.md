# helmを試す
context名: helm-tutorial-cluster

参考: https://github.com/cloudnativedevops/demo/tree/main/hello-helm

### クラスタの起動
$ kind create cluster --name helm-tutorial-cluster

## Helm

$ helm create demo
ディレクトリと各種ファイルが作られる
-> ただ使わないファイルも多いので、今回はほぼ削除して使った


$ helm install demo ./demo
(このディレクトリから実行)

$ helm uninstall demo

---
$ helm install demo-production --values=./demo/production-values.yaml ./demo


