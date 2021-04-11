# Flux Demo

This repository holds a demo of Flux v2.

## Things This Repository Deploys

1. An `ingress-nginx` Kubernetes ingress controller.
2. A set of infrastructure components.
    a. `prometheus-operator` for metrics collection and alerting.
    b. `grafana-loki` for log collection.
    c. `grafana` for metrics and log visualization.
3. A application webserver to test the whole setup.

## Repository Structure

```
bases/
  applications/
  infrastructure/
clusters/
  us-central1/
    test/
    stage/
    prod/
```

The `bases` holds the base application and infrastructure component declarations. The `clusters` folder hold the specific cluster configuration/overlays of both, the application and infrastructure components.