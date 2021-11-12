FROM debian:stable-slim

RUN apt-get update && apt-get install -y \
  wget \
  curl \
  libjansson4 \
 && rm -rf /var/lib/apt/lists/*

RUN mkdir cpuminer-gr && \
  cd cpuminer-gr && \
  wget https://github.com/michal-zurkowski/cpuminer-gr/releases/download/1.3.0/cpuminer-gr-aarch64-ubuntu18_04.tar.gz && \
  tar xvfz cpuminer-gr-aarch64-ubuntu18_04.tar.gz && \
  rm cpuminer-gr-aarch64-ubuntu18_04.tar.gz 

WORKDIR cpuminer-gr

CMD ./cpuminer-armv8 -a gr -o ${POOL} -u ${WALLET}

