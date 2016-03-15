# docker-adminer

[![ImageLayers Size](https://img.shields.io/imagelayers/image-size/activatedgeek/adminer/latest.svg)](https://hub.docker.com/r/activatedgeek/adminer/)

A docker image to run the lightweight `PHPMyAdmin` alternative called `Adminer`.
Learn more about Adminer [here](https://www.adminer.org).

## Images

* `latest`, `0.1`, `0.1.0` ([Dockerfile](./))

## Usage

Pull image from Docker hub as:
```
$ docker pull activatedgeek/adminer
```

This will pull the latest tag by default.

To run the container,
```
$ docker run -d -p 9090:80 \
  --name test-adminer \
  activatedgeek/adminer:latest
```

If you navigate to DOCKER_HOST:9090, you should see the adminer login page.

## Build

To build the image from source,
```
$ make latest
```