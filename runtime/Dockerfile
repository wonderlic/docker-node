FROM alpine:3.9
LABEL maintainer="Wonderlic DevOps <DevOps@wonderlic.com>"

RUN addgroup -g 1000 node \
    && adduser -u 1000 -G node -s /bin/sh -D node \
    && apk add --no-cache libstdc++

COPY --from=node:10.15.3-alpine /usr/local/bin/node /usr/local/bin
