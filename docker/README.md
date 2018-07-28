# Docker Setup

## Table of Contents

## Tutorials

[Official Docker Training][1] <br>
[Docker Startup][2]


## Adding Docker

Install
```
wget -qO- https://get.docker.com/ | sh
```

Test setup
```
sudo docker run hello-world
```

Setup user
```
sudo usermod -aG docker $USER
```
Note: you'll have to logout for this to take effect


[1]: https://training.docker.com/archive
[2]: https://docs.docker.com/get-started/

