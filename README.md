# Basic deployment server

A basic server made for deployment testing, such as nginx and port proxying

## How to use

- Mark ``index.js`` as an executable by doing ``chmod +x index.js``
- Copy your service file into the /etc/systemd/system.

- Start it with ``systemctl start basic_deploy``.