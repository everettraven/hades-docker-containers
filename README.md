# hades-docker-containers

This repository is all the Dockerfiles used to create the base images that hades uses to run its tests. Each Dockerfile is in a folder with the Operating System it uses.

Each image implements an OpenSSH Server that listens on port 22
The username and password used to login via SSH is: **root**

Feel free to build each of these images from source and use them as you see fit. You can also pull each of them from DockerHub by running:

```
docker pull bpalmer/<os>-base-ssh
```

Replace `<os>` with the desired operating system you would like the container to use.