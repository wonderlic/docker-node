FROM alpine:3.10
LABEL maintainer="Wonderlic DevOps <DevOps@wonderlic.com>"

RUN addgroup -g 1000 node \
	&& adduser -u 1000 -G node -s /bin/sh -D node

RUN apk add --no-cache nodejs
