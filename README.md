# Docker file for [Komoot Photon](https://github.com/komoot/photon)

### Building
```bash
docker build -t photon .
```

### Usage

To persist the storage a docker volume is recommended. Photon runs on port 2322 per default, this command will pipe it to port 443 on the host:

```bash
docker start -v photon_data:/data -p 443:2322  photon:latest
```
