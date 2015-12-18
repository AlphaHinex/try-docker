FROM debian:jessie

RUN apt-get update && apt-get install -y --no-install-recommends \
        curl \
        openssh-client 

ENV WD /usr/local/x
ENV URL http://screencasts.b0.upaiyun.com/podcasts/teahour_episode_78.m4a

WORKDIR $WD

RUN curl -fkSLO $URL 
