# GLASTOPF for Docker (alpine os)

[![Build Status](https://travis-ci.org/kTitan/docker-alpine-glastopf.svg)](https://travis-ci.org/kTitan/docker-alpine-glastopf)
[![Docker Stars](https://img.shields.io/docker/stars/ktitan/glastopf.svg)](https://hub.docker.com/r/ktitan/glastopf/)
[![Docker Pulls](https://img.shields.io/docker/pulls/ktitan/glastopf.svg)](https://hub.docker.com/r/ktitan/glastopf/)
[![ImageLayers Size](https://img.shields.io/imagelayers/image-size/ktitan/glastopf/latest.svg)](https://hub.docker.com/r/ktitan/glastopf/)
[![ImageLayers Layers](https://img.shields.io/imagelayers/layers/ktitan/glastopf/latest.svg)](https://hub.docker.com/r/ktitan/glastopf/)

Glastopf web application honeypot in a Docker container based on alpine linux.

## Upstream Links
* GitHub @ [kTitan/docker-alpine-glastopf](https://github.com/kTitan/docker-alpine-glastopf)
* GitHub @ [mushorg/glastopf](https://github.com/mushorg/glastopf)
* Docker @ [ktitan/glastopf](https://hub.docker.com/r/ktitan/glastopf/)

## Images Size

A short list with some of the current available glastopf docker images with their sizes
* [![size](https://img.shields.io/imagelayers/image-size/dtagdevsec/glastopf/latest.svg)](https://hub.docker.com/r/dtagdevsec/glastopf/) @ dtagdevsec
* [![size](https://img.shields.io/imagelayers/image-size/honeynet/glastopf/latest.svg)](https://hub.docker.com/r/honeynet/glastopf/) @ honeynet
* [![size](https://img.shields.io/imagelayers/image-size/tegonetworks/glastopf/latest.svg)](https://hub.docker.com/r/tegonetworks/glastopf/) @ tegonetworks
* [![size](https://img.shields.io/imagelayers/image-size/ktitan/glastopf/latest.svg)](https://hub.docker.com/r/ktitan/glastopf/) @ ktitan <- this image

## Usage

### Docker build
The Image is available as an automated build on docker hub.

```
docker pull ktitan/glastopf
```

### Docker Build
If you want to build the image on your own, here is an example for that.

```
docker build -t ktitan/glastopf:latest .
```

### Run
```
docker run -d -p 80:80 -v /data/glastopf:/opt/myhoneypot --name glastopf ktitan/glastopf
```
