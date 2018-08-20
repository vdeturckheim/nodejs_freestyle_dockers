FROM ubuntu:latest

RUN apt-get update
RUN apt-get install -y build-essential\
    git\
    curl

WORKDIR /root

ENV NVS_VERSION 1.2.0

RUN git clone --branch v$NVS_VERSION --depth 1 https://github.com/jasongin/nvs ~/.nvs
RUN echo '. ~/.nvs/nvs.sh' >> ~/.bashrc
RUN . ~/.nvs/nvs.sh
