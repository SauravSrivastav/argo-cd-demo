# argo-cd-demo
argo-cd-demo using helm chart



helm repo add argo https://argoproj.github.io/argo-helm

helm upgrade argocd argo/argo-cd --set server.service.type=LoadBalancer --namespace argo-system --install --create-namespace

helm uninstall argocd --namespace argo-system
