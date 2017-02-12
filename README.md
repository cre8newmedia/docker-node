# cre8/node

[Node](https://nodejs.org)JS [image](https://hub.docker.com/r/cre8/node/) that includes [yarn](https://yarnpkg.com).

## How to use this image

### Dockerfile

```Dockerfile
FROM cre8/node:latest

# [...]
```

### Docker-Compose

```yaml
version: '3'
services:
  
  app:
    image: cre8/node
    command: [yarn, run, start]
    working_dir: /usr/src/app
    volumes:
      - .:/usr/src/app
      - /usr/src/app/node_modules
```

## Build

Commit & push to [GitHub](https://github.com/cre8newmedia/docker-node)

It will automatically trigger build of new Docker Image.

Links:

- [Docker Cloud](https://cloud.docker.com/app/cre8/repository/docker/cre8/node/general)
- [Docker Hub](https://hub.docker.com/r/cre8/node/)

## License

MIT License
