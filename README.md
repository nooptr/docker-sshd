# How to install

Make a image for building container
```
docker build -t example/sshd .
```

Make a container from the docker image
```
docker run -it --name "sshd" -p 2222:22 -p 8080:80 example/sshd /bin/bash
```

Get ip of docker machine
```
$ docker-machine ip dev
192.168.99.100
```

To ssh from command line (user: root, password: root)
```
ssh -p 2222 root@192.168.99.100
```
