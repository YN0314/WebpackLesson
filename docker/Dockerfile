FROM node:current-alpine

ARG TZ

RUN set -eux && \
    apk add --update-cache --no-cache --virtual=.build-dependencies tzdata && \
    cp /usr/share/zoneinfo/${TZ} /etc/localtime && \
    apk add --update-cache npm yarn