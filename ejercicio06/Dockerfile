FROM registry.access.redhat.com/redhat-openjdk-18/openjdk18-openshift:1.12-1.1655301789
EXPOSE 8080
WORKDIR /app/
COPY passwordapi.jar /app/
CMD [ "java", "-jar", "/app/passwordapi.jar" ]