Docker Debian Systemd
=====================

This Dockerfile can build containers capable to use systemd.

Branches
--------

This repository has multiple branches that relate to Debian versions.

|Branch  |Debian Version    |Docker image tag|
|--------|------------------|----------------|
|master  |latest (buster/10)|latest          |
|testing |bullseye/sid      |testing         |
|unstable|bullseye/sid      |unstable        |

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
