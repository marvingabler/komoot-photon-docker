# Docker file for [Komoot Photon](https://github.com/komoot/photon)

### Building
```bash
docker build . -t photon
```

### Usage

To persist the storage a docker volume is recommended:

```bash
docker start -v photon_data:/data -p 443:2322  photon:latest
```