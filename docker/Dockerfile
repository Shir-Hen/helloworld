ARG REGISTRY=yann-sbx.dev.gcp.devopsacc.team
ARG DOCKER_REPO=urs-docker

#FROM $REGISTRY/$DOCKER_REPO/groovy:jre16
FROM java:8

# https://docs.docker.com/engine/reference/builder/#understand-how-arg-and-from-interact
# ARG REGISTRY

# dummy 
RUN mkdir -p /home/groovy/webapp/
COPY target/multi-module-application-2.0.0.jar /home/groovy/webapp/multi-module-application-2.0.0.jar

EXPOSE 8089

ENTRYPOINT ["java", "-jar", "/home/groovy/webapp/multi-module-application-2.0.0.jar"]