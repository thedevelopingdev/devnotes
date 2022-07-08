# Docker

## Writing `Dockerfile`s

Use `.dockerignore` to ignore particular files when using commands such as `COPY`.

## Running Docker containers

```shell
docker run -d -p <host>:<container> --rm --name <name> <image>:[tag]
```
