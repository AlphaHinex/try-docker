FROM tomcat:7
MAINTAINER Alpha Hinex <AlphaHinex@gmail.com>

ENV WEBAPP_HOME $CATALINA_HOME/webapps
RUN mkdir -p "$WEBAPP_HOME"
WORKDIR $WEBAPP_HOME

ENV WEBAPP_URL http://repo.gradle.org/gradle/libs/org/jasig/cas/cas-server-webapp/3.5.2/cas-server-webapp-3.5.2.war 

# Simply deploy war into webapps folder
RUN set -x \
        && curl -fSL "$WEBAPP_URL" -o cas-server.war
