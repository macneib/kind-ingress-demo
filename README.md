# kind-ingress-demo

## Steps to try

`kind create cluster --name hello-kind --config config.yaml`

`kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/kind/deploy.yaml`

`helm upgrade --install sre ./hello`

`curl -k -H 'Host:hello.sre.cts.enverus.dev' http://0.0.0.0 -v`

`kubectl port-forward services/sre-hello 8080:80 -n default`

`kind delete cluster --name hello-kind`
