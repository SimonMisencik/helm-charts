# job

A Helm chart for Kubernetes Job

## Get Repo Info

```console
helm repo add open https://simonmisencik.github.io/helm-charts
helm repo update
```

## Install Chart

```console
helm install [RELEASE_NAME] open/job
```

## Upgrading Chart

```console
helm upgrade [RELEASE_NAME] open/job
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
| `image.tag` | Image tag | `"latest"` |
| `imagePullSecrets` | Pull secrets for images | `[]` |
| `restartPolicy` | Restart policy for job container | `OnFailure` |
| `command` | Command for container | `'["bash", "-c", "sleep 365d"]'` |
| `extraInitContainers` | extraInitContainers for job | |
| `env` | Environment variables for job container | |
