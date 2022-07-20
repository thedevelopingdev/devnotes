# Docker

## Writing `Dockerfile`s

Use `.dockerignore` to ignore particular files when using commands such as `COPY`.

## Building Docker images

```shell
# multi-arch build
docker buildx build --platform=linux/amd64,linux/arm64 --push -t <name>:<tag> .
```

## Running Docker containers

```shell
docker run -d -p <host>:<container> --rm --name <name> <image>:[tag]
```
