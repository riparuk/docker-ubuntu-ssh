This is a simple ubuntu docker container that can be accessed using ssh.

## Install Docker
Visit the official [Docker](https://docs.docker.com/engine/install/) website and follow the installation instructions specific to your operating system.

## Clone this repository
```
git clone https://github.com/riparuk/docker-ubuntu-ssh.git
```

## Navigate to the repository directory containing the Dockerfile in terminal and do:
in Linux
```
cd docker-ubuntu-ssh
```

## Build the docker image
```
docker build -t docker-ubuntu-ssh
```

## Run the SSH Server Container
```
docker run -d -p 2626:22 docker-ubuntu-ssh
```
Change port `2626` to another if the port is in use

## SSH into the Container
Now you can SSH into the container with : 
```
ssh root@localhost -p 2626
```
default password is `123456`, you can change it as you wish by editing the Dockerfile. 


