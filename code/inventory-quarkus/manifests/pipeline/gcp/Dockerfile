# vim: set ft=Dockerfile
# derived from: https://github.com/GoogleCloudPlatform/cloud-build-samples/blob/main/maven-example/Dockerfile
# used for building the inventory app with Google Cloud Build

FROM openjdk:11

ARG JAR_FILE=JAR_FILE_MUST_BE_SPECIFIED_AS_BUILD_ARG

RUN find /

COPY ${JAR_FILE} app.jar

ENTRYPOINT ["java", "-Djava.security.edg=file:/dev/./urandom","-jar","/app.jar"]