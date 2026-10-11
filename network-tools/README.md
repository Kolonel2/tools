# network-tools

Minimal Ubuntu 26.04 image for debugging containers on Cycle.io.
Includes: curl, ping, ssh, plus ip, dig/nslookup, and nc.

## Local
    docker compose up -d --build
    docker compose exec network-tools bash

## Cycle.io
Create an image source of type "Docker Build" (or Dockerfile from Git) pointing at this repo,
build it, then deploy a container from it in your environment. Container runs `sleep infinity`;
use the Cycle console/instance shell to get in.
