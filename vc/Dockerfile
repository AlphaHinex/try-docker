FROM ubuntu:wily
MAINTAINER Alpha Hinex <AlphaHinex@gmail.com>
 
RUN apt-get update && apt-get -y install default-jdk ant git ffmpeg gpac libgpac-dev

ENV BASE /usr/local
WORKDIR $BASE
RUN git clone https://github.com/cablelabs/mse-eme.git

WORKDIR $BASE/mse-eme/create/encrypt
RUN ant clearkey

WORKDIR $BASE
