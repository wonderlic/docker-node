FROM node:10-buster-slim
LABEL maintainer="Wonderlic DevOps <DevOps@wonderlic.com>"

RUN apt-get update \
		&& apt-get install -y --no-install-recommends python2 make g++ gcc \
    && rm -rf /var/lib/apt/lists/*
