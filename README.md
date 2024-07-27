
# Helm Charts

## Introduction

This repository provides a set of Kubernetes manifests for deploying various resources, including deployments, services, and more. It is designed to be used as a base charts that can be extended and customized as needed.

## Updating Versions

### Update Chart Version

Whenever you make changes to the chart, update the `version` field in `Chart.yaml`:

```yaml
version: 0.2.0
```

### Update Image Tag

If the new version involves a new Docker image, update the `tag` field in `values.yaml`:

```yaml
image:
  tag: 1.1.0
```

### Version Control

Ensure you commit and push the changes to your version control system (e.g., Git):

```bash
git add Chart.yaml values.yaml
git commit -m "Updated chart and app version to 1.1.0"
git push origin main
```

## Best Practices

- Always increment the chart version in `Chart.yaml` with each change.
- Use semantic versioning for `version`.
- Keep your `values.yaml` file updated with the necessary configuration changes.
