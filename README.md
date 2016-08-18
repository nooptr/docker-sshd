# How to install

Make a image for building container
```
docker build -t example/sshd .
```

Make a container from the docker image
```
docker run -it --name "sshd" -p 2222:22 -p 8080:80 example/sshd /bin/bash
```
