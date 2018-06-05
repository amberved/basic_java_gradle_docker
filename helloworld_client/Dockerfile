#Build a container image with java jar using openjdk
#To build use "docker build -t myrepo/somename:latest --build-arg NAME="appname-1.0.jar ."

FROM openjdk:latest
ARG JAR_FILE

#RUN echo '***************************************'
RUN echo $JAR_FILE
#RUN echo '***************************************'

COPY $JAR_FILE app.jar
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "app.jar"]
