FROM weaveworksdemos/msd-java:jre-latest

WORKDIR /usr/src/app
COPY *.jar ./app.jar

ENTRYPOINT ["/usr/local/bin/java.sh", "-javaagent", "./dd-agent.jar", "-jar","./app.jar", "--port=80"]
