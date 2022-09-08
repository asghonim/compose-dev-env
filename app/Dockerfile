FROM docker/dev-environments-default:stable-1
RUN apt-get install curl
RUN curl -sL https://deb.nodesource.com/setup_14.x |  bash -
RUN apt-get install nodejs
RUN npm i -g local-web-server

RUN mkdir /com.docker.devenvironments.code
COPY .. /com.docker.devenvironments.code
WORKDIR /com.docker.devenvironments.code
RUN chown -R 1000:1000 /com.docker.devenvironments.code

USER 1000:1000

ENTRYPOINT ws
# FROM node:alpine
# RUN npm i -g local-web-server
# COPY ./index.html ./index.html
# CMD ws