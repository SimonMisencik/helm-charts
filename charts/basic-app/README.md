# basic-app

Basic-app helm chart for testing application/environment

## Get Repo Info

```console
helm repo add open https://simonmisencik.github.io/helm-charts
helm repo update
```

## Install Chart

```console
helm install [RELEASE_NAME] open/basic-app
```

## Upgrading Chart

```console
helm upgrade [RELEASE_NAME] open/basic-app
```

## Uninstall Chart

```console
helm uninstall [RELEASE_NAME]
```

## Configuration

| Parameter | Description | Default |
|-----------|-------------|---------|
| `replicaCount` | Number of nodes | `1` |
| `image.repository` | Image repository | `ovhplatform/what-is-my-pod` |
| `image.pullPolicy` | Image pull policy | `IfNotPresent` |
| `image.tag` | Image tag | `` |
| `image.port` | Image port | `8080` |
| `imagePullSecrets` | Image pull secrets | `[]` |
| `nameOverride` | Replaces the name of the chart in the Chart.yaml file | `""` |
| `fullnameOverride` |  Completely replaces the generated name | `""` |
| `service.type` | Kubernetes service type | `ClusterIP` |
| `service.port` | Kubernetes port where service is exposed | `80` |
| `ingress.enabled` | Enables Ingress | `false` |
| `ingress.annotations` | Ingress annotations (values are templated) | `{}` |
| `ingress.hosts` | Ingress accepted hostnames  | `[]` |
| `middleware.enabled` | Enable/disable traefik middleware resource | `false` |
| `middleware.stripPrefix` | stripPrefix value for traefik middleware | |
