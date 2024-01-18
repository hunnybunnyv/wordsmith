FROM ubuntu 
RUN apt-get update 
RUN apt-get install -y maven
COPY . .
RUN mvn verify
CMD ["java", "-Xmx8m", "-Xms8m", "-jar", "target/words.jar"]


#2eme facon
#FROM maven AS builder
#dependeces
#COPY pom.xml .
#RUN mvn verify

#build necessary or run container (sources)

#COPY src src
#RUN mvn verify

#FROM openjdk:8-jre-alpine

#COPY --from=builder target/ /target

#CMD exec java -Xmx8m -Xms8m -jar target/words.jar

