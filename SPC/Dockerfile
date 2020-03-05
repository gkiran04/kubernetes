FROM maven:3-jdk-8
LABEL author=KIRAN
RUN mkdir /usr/src/spc
WORKDIR /usr/src/spc
RUN git clone https://github.com/spring-projects/spring-petclinic.git && cd spring-petclinic && mvn clean package
EXPOSE 8080
ENTRYPOINT [ "java", "-jar", "/usr/src/spc/spring-petclinic/target/spring-petclinic-2.2.0.BUILD-SNAPSHOT.jar" ]
