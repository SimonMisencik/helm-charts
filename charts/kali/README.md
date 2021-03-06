# kali

Kali pod for penetration testing of cluster

## Get Repo Info

```console
helm repo add open https://simonmisencik.github.io/helm-charts
helm repo update
```

## Install Chart

```console
helm install [RELEASE_NAME] open/kali
```

## Upgrading Chart

```console
helm upgrade [RELEASE_NAME] open/kali
```

## Uninstall Chart

```console
helm uninstall [RELEASE_NAME]
```

## Configuration

| Parameter | Description | Default |
|-----------|-------------|---------|
| `image.repository` | Image repository | `kalilinux/kali-rolling` |
| `image.pullPolicy` | Image pull policy | `IfNotPresent` |
| `image.tag` | Image tag | `""` |
