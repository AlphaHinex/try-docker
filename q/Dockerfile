FROM debian:jessie

RUN apt-get update && apt-get install -y --no-install-recommends \
        curl \
        openssh-client 

ENV WD /usr/local/x
ENV URL https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/wro4j/wro4j-runner-1.6.3-jar-with-dependencies.jar 

WORKDIR $WD

RUN curl -fkSLO $URL 
