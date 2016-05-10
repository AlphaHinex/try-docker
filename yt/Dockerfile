FROM java:7-alpine
MAINTAINER Alpha Hinex <AlphaHinex@gmail.com>

RUN apk add --no-cache tzdata
RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
RUN echo "Asia/Shanghai" > /etc/timezone
RUN apk del tzdata

RUN wget http://download-cf.jetbrains.com/charisma/youtrack-6.5.17057.jar -O youtrack.jar

EXPOSE 80
CMD ["java", "-Xmx1g", "-XX:MaxPermSize=250m", "-Djava.awt.headless=true", "-jar", "youtrack.jar", "80/$CONTEXT_PATH"]
