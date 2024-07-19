# Redfish Exporter

This is a basic Kustomize definition for the Redfish-Exporter.

## Preparation

In order to make a Service Monitor work you have to add the Prometeus Operator CRDs:

```bash
kubectl apply -f https://github.com/prometheus-operator/prometheus-operator/releases/download/v0.73.2/stripped-down-crds.yaml
```

## Deployment

Deployment is done via the Kustomize apply command in `kubectl` or any other Kustomize compatible tool:

```bash
kubectl appky -k contrib/kustomize
```
