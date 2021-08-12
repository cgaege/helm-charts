# Averbis Kafka Helm Chart

This chart deploys Averbis Kafka in your Kubernetes cluster.

## Prerequisites

- A running Kubernetes cluster
- [Kubectl](https://kubernetes.io/docs/tasks/tools/)
- [Helm](https://helm.sh/docs/intro/install/)

## Creating Secret to pull Images

Create a secret named `averbis-docker-registry` with your Averbis credentials to pull images from the [Averbis docker registry](https://registry.averbis.com):

```
kubectl create secret docker-registry averbis-docker-registry \
--docker-server=https://registry.averbis.com \
--docker-username=me@example.com \
--docker-password=MySecretPassword
```

## Adding the Helm Repository
```
helm repo add averbis-charts https://cgaege.github.io/helm-charts/
helm repo update
```

## Installing the Chart

### Installing using Helm Repository
```
helm install my-release averbis-charts/kafka
```
### Installing using Chart Sources
```
helm install my-release .
```

## Upgrading the Chart
```
 helm upgrade my-release averbis-charts/kafka
```

## Uninstalling the Chart
```
helm uninstall my-release
```
