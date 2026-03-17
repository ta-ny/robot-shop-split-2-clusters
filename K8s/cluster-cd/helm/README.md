# Robot Shop - Cluster CD Helm Chart

This split Helm chart contains the **backend and async half** of Robot Shop.

## Included workloads
- payment
- shipping
- ratings
- dispatch
- mysql
- rabbitmq

## Notes
- This chart intentionally does **not** include Wallarm ingress resources.
- This half is intended to be deployed to **cluster-cd**.

## Install
```bash
helm install robot-shop-cd ./cluster-cd/helm
```
