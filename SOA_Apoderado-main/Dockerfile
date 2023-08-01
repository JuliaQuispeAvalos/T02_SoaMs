FROM alpine:latest

ENV JAVA_HOME="/usr/lib/jvm/default-jvm/"
RUN apk add openjdk17

ENV PATH=$PATH:${JAVA_HOME}/bin

CMD ["jshell"]

COPY target/Ms-apoderado-0.0.1-SNAPSHOT.jar /apoderados.jar

ENTRYPOINT ["java", "-jar", "/apoderados.jar"]

EXPOSE 8084
