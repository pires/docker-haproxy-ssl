# docker-haproxy-ssl
Lean (8MB) HAProxy + SSL termination Docker image, based on `progrium/busybox`.

[![Docker Repository on Quay.io](https://quay.io/repository/pires/docker-haproxy-ssl/status "Docker Repository on Quay.io")](https://quay.io/repository/pires/docker-haproxy-ssl)

## Current software

* HAProxy 1.5.11-patch02

## Pre-requisites

* Docker 1.5.0+ (tested with boot2docker)

## Run

```
docker run -d -p 80:80 -p 443:443 -v /path/to/your:/etc/haproxy/certs quay.io/pires/docker-haproxy-ssl:latest
```