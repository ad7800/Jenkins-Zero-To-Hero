# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM adoptopenjdk/openjdk16:jre16u-2021-09-25-01-21-beta-ubuntu-nightly

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
