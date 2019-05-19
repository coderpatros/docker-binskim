[![Build status](https://dev.azure.com/patros/OpenSource/_apis/build/status/docker-binskim)](https://dev.azure.com/patros/OpenSource/_build/latest?definitionId=24)
![Docker Pulls](https://img.shields.io/docker/pulls/coderpatros/binskim.svg)

BinSkim Docker Container
========================

_PLEASE NOTE: I am currently using a custom build of BinSkim._

The official build hasn't been updated in a while.
I'm not making any changes, just taking the latest master branch from the [offical repository](https://github.com/microsoft/binskim).

Basic Usage
-----------

Running (assuming binaries are in the current working directory)...

    docker run --user `id --user`:`id --user` --volume `pwd`:/code coderpatros/binskim analyze /code/*.dll --recurse --output /code/binskim.sarif

Docker Tags
-----------

Current tag to track is `latest`.

I regularly rebuild the image to ensure it picks up any updates to the base `ubuntu:18.04` image and the official repository.
