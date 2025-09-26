# ProteinMPNN

### Build ProteinMPNN docker image.

```sh
docker build -t proteinmpnn:fastapi -f docker/Dockerfile .
```

### Save ProteinMPNN docker image.

```sh
docker save proteinmpnn:fastapi | gzip > docker_images/proteinmpnn_fastapi.tar.gz
```


