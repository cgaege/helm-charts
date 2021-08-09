# Averbis Helm Charts

Helm charts to deploy Averbis applications in your Kubernetes cluster.

## Prerequisites
- A running Kubernetes cluster
- Helm 3.x


```
$ helm repo add averbis-charts https://cgaege.github.io/helm-charts
$ helm search repo averbis-charts
$ helm install my-release averbis-charts/<chart>
```