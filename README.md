# Installation

## Deployment cert-manager

1. Add the Helm Repository & Update
```bash
helm repo add jetstack https://charts.jetstack.io

helm repo update
```
2. Install Cert-Manager with Helm & CRDs
```bash
helm install cert-manager jetstack/cert-manager --namespace cert-manager --create-namespace --set installCRDs=true
```

## Expose traefik dashboard

https://stackoverflow.com/questions/68565048/how-to-expose-traefik-v2-dashboard-in-k3d-k3s-via-configuration
