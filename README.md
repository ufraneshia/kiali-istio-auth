**write read me later**

```
helm repo add https://istio-release.storage.googleapis.com/charts
helm repo add kiali https://kiali.org/helm-charts
helm repo update
helm dependency build
helm package .
helm repo index .
```

## Addendum
GitHub source repo URL is not a valid Helm chart repository.
Helm needs a static HTTP server that serves index.yaml and .tgz files — GitHub Pages provides that, but a normal GitHub repo does not.

Enable GitHub Pages

`Settings → Pages → Source: gh-pages → / (root)`

Your published repo will now be available at:

`https://myname.github.io/myrepo/`