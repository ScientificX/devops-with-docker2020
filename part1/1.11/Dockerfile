FROM ubuntu:16.04

RUN apt-get -y update && apt-get -y upgrade

RUN apt-get install -y git

RUN apt-get install -y curl

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash

RUN apt install -y nodejs

RUN git clone https://github.com/docker-hy/backend-example-docker.git /backend

WORKDIR /backend

RUN npm i

EXPOSE 8000

CMD ["/bin/bash"]
