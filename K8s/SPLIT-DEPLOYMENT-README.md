# Split Robot Shop Deployment

This package splits Robot Shop into two Helm charts so the application can be deployed across two clusters.

## Cluster AB
Entry/front-facing services:
- web
- catalogue
- user
- cart
- mongodb
- redis
- Wallarm ingress resources

## Cluster CD
Backend/async services:
- payment
- shipping
- ratings
- dispatch
- mysql
- rabbitmq

## Folder layout
- cluster-ab/helm
- cluster-cd/helm

## Wallarm IP allowlist retained in cluster-ab
- 65.132.246.78/32
- 112.216.0.186/32
