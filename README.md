# kind-ingress-demo

## Steps to try

`kind create cluster --name hello-kind --config config.yaml`

`kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/kind/deploy.yaml`

`helm upgrade --install sre ./hello`

`kind delete cluster --name hello-kind`
