FROM java:8-jre
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/node-sidecar-0.0.1-SNAPSHOT.jar /app/
CMD ["java", "-Xmx200m", "-jar", "/app/node-sidecar-0.0.1-SNAPSHOT.jar"]

EXPOSE 8741