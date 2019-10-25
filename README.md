# wonderlic/node

### Links

* github: [https://github.com/wonderlic/docker-node](https://github.com/wonderlic/docker-node)
* docker hub: [https://registry.hub.docker.com/u/wonderlic/node/](https://registry.hub.docker.com/u/wonderlic/node/)

### alpine

#### 10-alpine

This is a minimal docker image based on the root alpine:3.9 image with just enough added to be able to run the node executable.
It does not contain npm or any dev tools.
It is meant to be used as the base image for the release portion of a docker multistage build.
It will need to have the node application code (including the already build node_modules) copied to it.

Major Versions:
	Alpine 3.9 (https://wiki.alpinelinux.org/wiki/Alpine_Linux:Releases)
	Node v10 LTS (i.e Dubnium - https://nodejs.org/en/about/releases/)

#### 10-alpine-builder

This is a docker image based on node:10-alpine that contains node, npm, and a few common dev tools that are needed by npm to build the node_modules directory.
It is not meant to be used at runtime.
Instead, it is meant to be used for the build portion of a docker multistage build.

### buster-slim

#### 10-buster-slim

This is a minimal docker image based on the root debian:buster-slim image with just enough added to be able to run the node executable.
It does not contain npm or any dev tools.
It is meant to be used as the base image for the release portion of a docker multistage build.
It will need to have the node application code (including the already build node_modules) copied to it.

Major Versions:
	Debian 10 Stable (i.e. Buster - https://www.debian.org/releases/)
	Node v10 LTS (i.e Dubnium - https://nodejs.org/en/about/releases/)

#### 10-buster-slim-builder

This is a docker image based on node:10-buster-slim that contains node, npm, and a few common dev tools that are needed by npm to build the node_modules directory.
It is not meant to be used at runtime.
Instead, it is meant to be used for the build portion of a docker multistage build.
