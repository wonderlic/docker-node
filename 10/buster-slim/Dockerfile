FROM debian:buster-slim
LABEL maintainer="Wonderlic DevOps <DevOps@wonderlic.com>"

RUN groupadd --gid 1000 node \
		&& useradd --uid 1000 --gid node --shell /bin/bash --create-home node

COPY --from=node:10-buster-slim /usr/local/bin/node /usr/local/bin
