FROM openjdk:8u131-jdk

MAINTAINER JasonLu <raylupus@gmail.com>

RUN mkdir -p /mnt/data/apps

EXPOSE 8000
ENV VERSION=1.0.0
ENV JAVA_OPTS="-Xmx256m -Xms256m"

ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -jar /mnt/data/apps/spring-eureka-server-${VERSION}.jar" ]

ADD spring-eureka-server-${VERSION}.jar /mnt/data/apps