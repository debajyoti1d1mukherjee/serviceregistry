FROM java:8
VOLUME /tmp
ADD configserver-0.0.1-SNAPSHOT.jar configserver-0.0.1-SNAPSHOT.jar
RUN sh -c 'touch /configserver-0.0.1-SNAPSHOT.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /configserver-0.0.1-SNAPSHOT.jar" ]
