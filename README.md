# resources

## Tricks

Build
```shell
docker run -u "$(id -u):$(id -g)" -v $PWD:/app --workdir /app ghcr.io/getzola/zola:v0.19.2 build
```

Run at [localhost:8181](https://localhost:8181)
```shell
docker run -u "$(id -u):$(id -g)" -v $PWD:/app --workdir /app -p 8181:8181 ghcr.io/getzola/zola:v0.19.2 serve --interface 0.0.0.0 --port 8181 --base-url localhost
```

