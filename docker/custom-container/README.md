# Simple custom container

## Purpose
* Build a simple server container that can be interacted with locally
* Use a Linux base image (Ubuntu) where we have to install some packages on demand (Ruby)
* Install Bundler and install some gems on demand
* Publish image to DockerHub

## Details
* [Public Docker Image](https://hub.docker.com/r/jhong97/simple_rackup_server)
* Rackup server can also run locally on port 9292 via ```rackup -p 9292```
  * Interact at ```localhost:9292```
* Run in container using ```docker run -p 0.0.0.0:9292:9292 <container-id>```
  * Interact at ```0.0.0.0:9292```
