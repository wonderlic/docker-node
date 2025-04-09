FROM node:20.19-alpine3.21 as staging

RUN apk --no-cache add binutils

RUN strip -s /usr/local/bin/node

#---------------------------------------------------------------------
FROM alpine:3.21
LABEL maintainer="Wonderlic DevOps <DevOps@wonderlic.com>"

RUN addgroup -g 1000 node \
	&& adduser -u 1000 -G node -s /bin/sh -D node \
	&& apk --no-cache add libstdc++

COPY --from=staging /usr/local/bin/node /usr/local/bin/
