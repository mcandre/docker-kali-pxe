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

## Debian/Ubuntu

```
$ sudo apt-get install docker.io qemu
```

## RedHat/Fedora/CentOS

```
$ sudo yum install docker-io qemu
```

## non-Linux

* [VirtualBox](https://www.virtualbox.org/)
* [Docker Toolbox](https://www.docker.com/toolbox)

### Mac OS X

* [Xcode](http://itunes.apple.com/us/app/xcode/id497799835?ls=1&mt=12)
* [Homebrew](http://brew.sh/)
* [brew-cask](http://caskroom.io/)

```
$ brew cask install dockertoolbox
```

### Windows

* [Chocolatey](https://chocolatey.org/)

```
> chocolatey install virtualbox make
```

* [DockerToolbox-1.8.2c.exe](https://github.com/docker/toolbox/releases/download/v1.8.2c/DockerToolbox-1.8.2c.exe)
