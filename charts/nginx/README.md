# nginx

nginx pod for penetration nginxing of cluster

## Get Repo Info

```console
helm repo add open https://simonmisencik.github.io/helm-charts
helm repo update
```

## Install Chart

```console
helm install [RELEASE_NAME] open/nginx
```

## Upgrading Chart

```console
helm upgrade [RELEASE_NAME] open/nginx
```

## Uninstall Chart

```console
helm uninstall [RELEASE_NAME]
```

## Configuration

| Parameter | Description | Default |
|-----------|-------------|---------|
| `image.repository` | Image repository | `nginx` |
| `image.pullPolicy` | Image pull policy | `IfNotPresent` |
| `image.tag` | Image tag | `""` |
