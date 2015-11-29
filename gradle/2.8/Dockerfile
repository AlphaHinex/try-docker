FROM java:7
MAINTAINER Alpha Hinex <AlphaHinex@gmail.com>

ENV WEBAPP_NAME arsenal
ENV WEBAPP_HOME /usr/local/webapps
RUN mkdir -p "$WEBAPP_HOME"
WORKDIR $WEBAPP_HOME

ENV WEBAPP_URL https://github.com/AlphaHinex/arsenal.git 

RUN git clone $WEBAPP_URL

WORKDIR $WEBAPP_HOME/$WEBAPP_NAME
RUN ./gradlew check

CMD set -x \
        && git pull \
        && ./gradlew clean check \
        && cd build/reports/tests \
        && python -m SimpleHTTPServer 8080
