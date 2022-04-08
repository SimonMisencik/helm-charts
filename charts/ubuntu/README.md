# ubuntu

Ubuntu pod for testing or debugging with tools:
- curl
- nmap
- postgresql-client

## Get Repo Info

```console
helm repo add open https://simonmisencik.github.io/helm-charts
helm repo update
```

## Install Chart

```console
helm install [RELEASE_NAME] open/ubuntu
```

## Upgrading Chart

```console
helm upgrade [RELEASE_NAME] open/ubuntu
```

## Uninstall Chart

```console
helm uninstall [RELEASE_NAME]
```

## Configuration

| Parameter | Description | Default |
|-----------|-------------|---------|
| `image.repository` | Image repository | `ubuntu` |
| `image.pullPolicy` | Image pull policy | `IfNotPresent` |
| `image.tag` | Image tag | `""` |
