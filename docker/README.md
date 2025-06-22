# ProteinMPNN

### Build ProteinMPNN docker image.

```sh
docker build -t ProteinMPNN:cli -f docker/Dockerfile .
```

### Save ProteinMPNN docker image.

```sh
docker save ProteinMPNN:cli | gzip > docker_images/ProteinMPNN_cli.tar.gz
```

