# docker-kali-pxe - a Docker container running a continuous PXE server for Kali Linux

# DOCKER HUB

https://registry.hub.docker.com/u/mcandre/docker-kali-pxe/

# EXAMPLE

```
$ docker run -d -p 69:69/udp --cap-add=NET_ADMIN mcandre/docker-kali-pxe
$ qemu-system-x86_64 -no-acpi -boot n -bootp tftp://$(docker-machine ip default)/pxelinux.0
```

# REQUIREMENTS

* [Docker](https://www.docker.com/)
* [qemu](http://wiki.qemu.org/Main_Page)

## Optional

* [make](http://www.gnu.org/software/make/)
* [Node.js](https://nodejs.org/en/) (for dockerlint)
