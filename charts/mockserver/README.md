# mockserver

mockserver helm chart for deployment of mockserver

## Get Repo Info

```console
helm repo add open https://simonmisencik.github.io/helm-charts
helm repo update
```

## Install Chart

```console
helm install [RELEASE_NAME] open/mockserver
```

## Upgrading Chart

```console
helm upgrade [RELEASE_NAME] open/mockserver
```

## Uninstall Chart

```console
helm uninstall [RELEASE_NAME]
```

## Configuration

| Parameter | Description | Default |
|-----------|-------------|---------|
| `replicaCount` | Number of nodes | `1` |
| `image.repository` | Image repository | `mockserver/mockserver` |
| `image.pullPolicy` | Image pull policy | `IfNotPresent` |
| `image.tag` | Image tag | `` |
| `imagePullSecrets` | Image pull secrets | `[]` |
| `nameOverride` | Replaces the name of the chart in the Chart.yaml file | `""` |
| `fullnameOverride` |  Completely replaces the generated name | `""` |
| `service.type` | Kubernetes service type | `ClusterIP` |
| `service.port` | Kubernetes port where service is exposed | `1080` |
| `service.containerPort` | Kubernetes container port | `1080` |
| `ingress.enabled` | Enables Ingress | `false` |
| `ingress.annotations` | Ingress annotations (values are templated) | `{}` |
| `ingress.hosts` | Ingress accepted hostnames  | `[]` |
| `extraEnv` | Specification of env variables  | `[]` |
