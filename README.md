Docker Debian Systemd
=====================

This Dockerfile can build containers capable to use systemd.

[![debian build status](https://img.shields.io/docker/cloud/build/robertdebock/debian.svg)](https://hub.docker.com/repository/docker/robertdebock/debian)

Branches
--------

This repository has multiple branches that relate to Debian versions.

|Branch  |Debian Version      |Docker image tag|
|--------|--------------------|----------------|
|master  |latest (bookworm/12)|latest          |
|bullseye|bullseye (11)       |bullseye        |
|buster  |buster (10)         |buster          |

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```
docker run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  robertdebock/debian
```
