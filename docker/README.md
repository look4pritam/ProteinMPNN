# ProteinMPNN

### Build ProteinMPNN docker image.

```sh
docker build -t proteinmpnn:cli -f docker/Dockerfile .
```

### Save ProteinMPNN docker image.

```sh
docker save proteinmpnn:cli | gzip > docker_images/proteinmpnn_cli.tar.gz
```

