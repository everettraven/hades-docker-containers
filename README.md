# hades-docker-containers

This repository is all the Containerfiles used to create the base images that hades uses to run its tests. Each Containerfile is in a folder with the Operating System it uses. 

*NOTE: Podman is used to build and run these containers to run systemd within the containers. Using Docker normally will likely not work and would likely require mounting the host systems systemd*

Each image implements an OpenSSH Server that listens on port 22
The username and password used to login via SSH is: **root**

Feel free to build each of these images from source and use them as you see fit. You can also pull each of them from DockerHub by running:

```
podman pull bpalmer/<os>-base-ssh
```

Replace `<os>` with the desired operating system you would like the container to use.