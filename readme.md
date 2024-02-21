# Kustomize + argocd deployment files for [k8s-hello-server](https://github.com/fokot/k8s-hello-server)

We have two environments `am` and `pigs`.

Run build kustomization for environment like
```
kustomize build overlays/am
```

or
```
kubectl kustomize overlays/am
```

`Kustomize` does not have good documentation, best is to look to [examples](https://github.com/kubernetes-sigs/kustomize/tree/master/examples).

`<am-secret-replaced>` will be replaced by [ArgoCD parameter overrides](https://argo-cd.readthedocs.io/en/stable/user-guide/parameters/) or maybe not
