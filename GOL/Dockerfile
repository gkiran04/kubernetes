FROM maven:3-jdk-8 as gol
LABEL author=KIRAN
RUN git clone https://github.com/wakaleo/game-of-life.git && cd game-of-life && mvn clean install

FROM tomcat:8
LABEL author=KIRAN
COPY --from=gol /game-of-life/gameoflife-web/target/gameoflife.war /usr/local/tomcat/webapps/gameoflife.war
EXPOSE 8080
CMD ["catalina.sh", "run"]