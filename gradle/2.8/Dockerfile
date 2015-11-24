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

CMD git pull
CMD ./gradlew check 
CMD python -m SimpleHTTPServer 8080 build/reports/tests/
