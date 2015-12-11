FROM debian:jessie

RUN apt-get update && apt-get install -y --no-install-recommends \
        curl \
        openssh-client 

ENV WD /usr/local/x
ENV URL https://github.com/github/git-lfs/releases/download/v1.1.0/git-lfs-darwin-amd64-1.1.0.tar.gz

WORKDIR $WD

RUN curl -O $URL 
