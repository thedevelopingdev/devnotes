# Kubernetes

## Usability tricks
```
# .zshrc

source <(kubectl completion zsh)
```


## Creating secrets

```shell
# from env file, e.g. .env.local
# source: https://archive.ph/46UEE

kubectl create secret generic <secretName> --from-env-file=<file>

# read secret
kubectl get secret <SECRET_NAME> -o jsonpath="{.data.<DATA>}" | base64 --decode
```

## Use secrets

```yaml
envFrom:
  - secretsRef:
      name: <secret name>
```

## Execute commands in pod

```shell
# single command
kubectl exec <POD_NAME> -- <command>

# interactive shell (/bin/bash is generally not available)
kubectl exec -it <POD_NAME> [-c <CONTAINER>] -- /bin/sh
```

## Create debugging pod
 - source: https://archive.ph/Miwsz
