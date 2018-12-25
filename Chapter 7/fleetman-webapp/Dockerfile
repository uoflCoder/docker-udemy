FROM tomcat:8.5.16-jre8-alpine

MAINTAINER Tylor Cornett "tylorcornett@gmail.com"

EXPOSE 8080

RUN rm -rf /usr/local/tomcat/webapps/*

COPY ./target/fleetman-0.0.1-SNAPSHOT.war /usr/local/tomcat/webapps/ROOT.war

ENV JAVA_OPTS="-Dspring.profiles.active=development"

CMD ["catalina.sh", "run"]