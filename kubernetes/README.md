# Kubernetes

## Creating secrets

```shell
# from env file, e.g. .env.local

kubectl create secret generic <secretName> --from-env-file=<file>
```
