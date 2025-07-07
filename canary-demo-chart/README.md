# Canary Demo Helm Chart

## Installation
```bash
helm install canary-demo ./canary-demo-chart
```

## Upgrade (Trigger Canary)
```bash
helm upgrade canary-demo ./canary-demo-chart --set app.tag=v2
```

## Uninstall
```bash
helm uninstall canary-demo
```

## Access Grafana
```bash
kubectl port-forward svc/grafana -n grafana 3000:80
```