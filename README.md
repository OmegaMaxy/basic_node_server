# Basic deployment server

A basic server made for deployment testing, such as nginx and port proxying

## How to use

- Mark ``index.js`` as an executable by doing ``chmod +x index.js``
- Copy your service file into the /etc/systemd/system.

- Start it with ``systemctl start basic_deploy``.

## Docker deployment

Build your image with the name ``basic-node-server``.
This command will look at the Dockerfile for instructions.
```
docker build -t basic-node-server .
```

Create and run a container based of the image ``basic-node-server``.
We've assigned the the container port 3000 to the host port 3000 ``host:container``.
```
docker run -p 3000:3000 basic-node-server
```
