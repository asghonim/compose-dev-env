FROM docker/dev-environments-default:stable-1
RUN apt-get install curl
RUN curl -sL https://deb.nodesource.com/setup_14.x |  bash -
RUN apt-get install nodejs
RUN npm i -g local-web-server

USER 1000:1000
# RUN mkdir /home/vscode/project
# WORKDIR /home/vscode/project
ENTRYPOINT ws
# FROM node:alpine
# RUN npm i -g local-web-server
# COPY ./index.html ./index.html
# CMD ws