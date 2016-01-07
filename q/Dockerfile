FROM debian:jessie

RUN apt-get update && apt-get install -y --no-install-recommends \
        curl \
        openssh-client 

ENV WD /usr/local/x
ENV URL https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-1.9.8-macosx.zip 

WORKDIR $WD

RUN curl -fkSLO $URL 
