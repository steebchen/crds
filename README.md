# YAML Manifests Collection

This repository contains a collection of combined YAML manifests from various sources, organized for easy use and reference. Currently, it includes:

1. GCP Config Connector - Combined Custom Resource Definitions (CRDs)

More manifest collections will be added in the future.

## How It Works

GitHub Actions workflows run on a schedule to:

1. Clone source repositories
2. Find and process YAML files
3. Combine them into single YAML files with proper separators (`---`)
4. Push the combined files to this repository

## Available Manifests

### Using with IntelliJ IDEA

You can add the CRD specifications to IntelliJ IDEA for validation and code completion:

1. Go to Settings → Languages & Frameworks → Kubernetes
2. Under the "External specifications" section, click the "+" button
3. Add the combined CRDs file from this repository using the URLs below

### GCP Config Connector

The combined CRDs file for Google Cloud Platform Kubernetes Config Connector is available at:

```
outputs/gcp/configconnector.yaml
```

Full URL:

```
https://github.com/steebchen/yaml-manifests/blob/main/outputs/gcp/configconnector.yaml
```

## Manual Trigger

You can manually trigger any workflow by:

1. Going to the "Actions" tab in this repository
2. Selecting the desired workflow
3. Clicking "Run workflow"

## License

This repository is provided under the same license as the original [k8s-config-connector](https://github.com/GoogleCloudPlatform/k8s-config-connector) repository.
