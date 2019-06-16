FROM node:8
MAINTAINER Martin Taheri <m3hran@gmail.com>
LABEL Description="AoT-backend Image"

    
RUN mkdir -p /u/apps && cd /u/apps && \
    git clone https://github.com/triestpa/Atlas-Of-Thrones.git

RUN cd /u/apps/Atlas-Of-Thrones && npm install

WORKDIR /u/apps/Atlas-Of-Thrones
EXPOSE 5000
ENTRYPOINT  NODE_ENV=local npm start