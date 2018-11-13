FROM node:8.12.0-alpine

WORKDIR /app

RUN apk update && \
    apk add git && \
    npm install -g npm && \
    npm install -g vue-cli

#CMD ["/bin/sh"]