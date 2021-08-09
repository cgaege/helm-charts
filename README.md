# Averbis Helm Charts

Helm charts to deploy Averbis applications in your Kubernetes cluster.

## Prerequisites
- A running Kubernetes cluster
- Helm 3.x

## Installing Helm
Helm is a package manager for Kubernetes. Helm Charts are packages of pre-configured Kubernetes resources.

To install Helm, refer to the [Helm install guide](https://helm.sh/docs/intro/install/).

```
$ helm repo add averbis-charts https://cgaege.github.io/helm-charts
$ helm search repo averbis-charts
$ helm install my-release averbis-charts/<chart>
```