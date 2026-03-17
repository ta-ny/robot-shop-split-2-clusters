# Robot Shop - Cluster AB Helm Chart

This split Helm chart contains the **entry and front-facing half** of Robot Shop.

## Included workloads
- web
- catalogue
- user
- cart
- mongodb
- redis
- wallarm-ingress
- wallarm-ingress-controller service

## Notes
- This chart retains the Wallarm ingress resources.
- The allowed IPs remain:
  - 65.132.246.78/32
  - 112.216.0.186/32
- This half is intended to be deployed to **cluster-ab**.

## Install
```bash
helm install robot-shop-ab ./cluster-ab/helm
```
