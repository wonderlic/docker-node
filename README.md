# wonderlic/node

### Links

* github: [https://github.com/wonderlic/docker-node](https://github.com/wonderlic/docker-node)
* docker hub: [https://registry.hub.docker.com/u/wonderlic/node/](https://registry.hub.docker.com/u/wonderlic/node/)

### Tags

#### [NODE_VER]-build

This is a docker image based on node:NODE_VER-alpine that contains node, npm, and a few common dev tools that are needed by npm to build the node_modules directory.
It is not meant to be used at runtime.
Instead, it is meant to be used for the build portion of a docker multistage build.

#### [NODE_VER]-runtime

This is a minimal docker image based on the root alpine:VER image with just enough added to be able to run the node executable.
It does not contain npm or any dev tools.
It is meant to be used as the base image for the release portion of a docker multistage build.
It will need to have the node application code (including the already build node_modules) copied to it.
