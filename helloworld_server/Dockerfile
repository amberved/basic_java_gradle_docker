FROM openjdk:latest
ARG JAR_FILE
#RUN echo '***************************************'
RUN echo $JAR_FILE
#RUN echo '***************************************'
COPY $JAR_FILE app.jar
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "app.jar"]