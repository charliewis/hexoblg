---
title: Docker Notes
date: 2021-08-13 09:36:16
tags:
---

### build
```
docker build -t docker_name .
```

### e.g.
```
docker build -t u16.04:ubuntu .
```

### view image
```
docker images
```

### remove image
```
docker image rm <docker_name>
```

### save and load to another computer
```
docker save apache2:latest > apache2.tar
scp ...
docker load -i apache2.tar
```

### run
```
#!/bin/sh
    APACHE2_HOME=<volumn top path>
    docker run --rm -itd \
    --name <container_name> \
    -p <host_port>:80 \
    -v $APACHE2_HOME/www:/var/www \
    -v $APACHE2_HOME/etc/apache2:/etc/apache2 \
    <docker_name>
```
### view containers
```
docker ps
```

### exec
```
docker exec -it <container_name> /bin/bash
```

### stop
```
docker stop <container_name>
```

### remove container
```
docker rm <container_name>
```

### remove image
```
docker rmi <image_name>
```

---
### setup
```
sudo  apt install docker.io
```
---
```
curl -sf -L https://static.rust-lang.org/rustup.sh -o rustup.sh
less rustup.sh
chmod +x rustup.sh
sudo ./rustup.sh
source $HOME/.cargo/env
source $HOME/.bashrc
```

## add to docker group
```
sudo usermod -aG docker charlie
```

## restart
```
sudo service docker restart
```

## reboot

## view version
```
docker version
```



