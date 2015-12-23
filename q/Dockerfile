FROM debian:jessie

RUN apt-get update && apt-get install -y --no-install-recommends \
        curl \
        openssh-client 

ENV WD /usr/local/x
ENV URL https://dl.google.com/chrome/win/9559FFD4C2CF2E2F/46.0.2490.86_chrome_installer.exe 

WORKDIR $WD

RUN curl -fkSLO $URL 
