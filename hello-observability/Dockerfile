FROM openjdk:17-ea-jdk-slim-buster
EXPOSE 8080
ARG JAR=hello-observability.jar
COPY target/$JAR /app.jar
COPY opentelemetry-javaagent.jar /opentelemetry-javaagent.jar
ENTRYPOINT ["java","-jar","/app.jar"]