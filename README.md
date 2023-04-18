# NMS Docker Lab Environment

NGINX Management Suite Docker Lab

The Docker Compose file will build the NGINX container if it is not already chanced on your system.
`Note:` You will need to have `NMS` and `Clickhouse` running to build the container correctly.

## Dependencies

You will need:

- NGINX Repository certificate and key
- NMS license
- Docker

You will need to set the following variables in a `.env` file:

- DOCKER_REGISTRY="your container registry"
- NIM_LICENSE="your nim license in a base64 format"

## Build NGINX Container

```bash
docker compose up -d nms clickhouse echo
docker compose up -d nginx-plus
```

## Start Lab Environment

```bash
docker compose up -d
```
