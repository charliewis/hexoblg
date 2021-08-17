---
title: Docker Notes
date: 2021-08-13 09:36:16
tags:
---

### build
**docker build -t *docker_name* .**
### e.g.```
docker build -t u16.04:ubuntu .
```

### save and load to another computer
```
docker save apache2:latest > apache2.tar
scp ...
docker load -i apache2.tar
```