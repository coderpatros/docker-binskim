![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/coderpatros/binskim)
![Docker Pulls](https://img.shields.io/docker/pulls/coderpatros/binskim.svg)
[![](https://images.microbadger.com/badges/image/coderpatros/binskim.svg)](https://microbadger.com/images/coderpatros/binskim "Get your own image badge on microbadger.com")
![GitHub](https://img.shields.io/github/license/patros/docker-binskim)

BinSkim Docker Container
========================

_PLEASE NOTE: I am currently using a custom build of BinSkim._

The official build hasn't been updated in a while.
I'm not making any changes, just taking the latest master branch from the [offical repository](https://github.com/microsoft/binskim).

Basic Usage
-----------

Running (assuming binaries are in the current working directory)...

    docker run --user `id --user`:`id --user` --volume `pwd`:/code coderpatros/binskim analyze /code/*.dll --recurse --output /code/binskim.sarif

More Documentation
------------------

Please refer to the [official repository](https://github.com/microsoft/binskim) for more documentation.

Docker Tags
-----------

Current tag to track is `latest`.

I regularly rebuild the image to ensure it picks up any updates to the base `ubuntu:18.04` image and the official repository.
