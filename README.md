# === SSH tutorial === #
https://www.youtube.com/watch?v=8X4u9sca3Io 

# === TLS tutorial === #
https://docs.bitnami.com/tutorials/secure-kubernetes-services-with-ingress-tls-letsencrypt

# === ArgoCD tutorial === #
https://argo-cd.readthedocs.io/en/stable/getting_started/

# === Adding ArgoCD === #
kubectl apply -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/core-install.yaml

# === DNS URI === #
https://meirapp.ddns.net/

# === Github repo === #
git@github.com:shay1987/demo-crm-argocd.git

# === ArgoCD UI === #
3.kubectl port-forward svc/argocd-server 8080:443

<!-- apiVersion: argoproj.io/v1alpha1
kind: Application
metadata:
  name: demo-crm
  namespace: argocd
spec:
  project: default
  source:
    repoURL: git@github.com:amitzarmon/demo-crm-argocd.git
    path: amit-demo-crm
  destination:
    server: https://kubernetes.default.svc
    namespace: default

  syncPolicy:
    syncOptions:
    - CreateNamespace=true

    automated:
      selfHeal: true
      prune: true -->