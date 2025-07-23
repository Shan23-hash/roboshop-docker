 FROM maven
 WORKDIR /opt/server
 COPY pom.xml .
 COPY src /opt/server/src
 RUN mvn clean package \