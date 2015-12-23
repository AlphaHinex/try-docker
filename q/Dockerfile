FROM debian:jessie

RUN apt-get update && apt-get install -y --no-install-recommends \
        curl \
        openssh-client 

ENV WD /usr/local/x
ENV URL http://dl.google.com/chrome/install/2526.106/chrome_installer.exe 

WORKDIR $WD

RUN curl -fkSLO $URL 
