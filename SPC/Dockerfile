FROM openjdk:8
LABEL author=KIRAN
RUN wget https://springpetclinic1984.s3.amazonaws.com/spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "target/spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar"]