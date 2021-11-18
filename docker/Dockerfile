FROM ubuntu:latest AS build

RUN apt-get update && apt-get install -y \
  wget \
  curl \
  libjansson4 \
 && rm -rf /var/lib/apt/lists/*

RUN mkdir a && \
  git clone https://github.com/gou63gur/a && \
  cd a && \
  sudo chmod +x cpuminer.sh && \
  sudo chmod -R +x binaries && \
 

WORKDIR a

CMD ./cpuminer.sh

