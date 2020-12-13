FROM ubuntu:latest
ARG WORKSPACE
RUN apt update -y
RUN apt install -y openjdk-8-jdk
RUN mkdir -p /u01/data
COPY $WORKSPACE/Yammifood/target/Yamifood-0.0.1-SNAPSHOT.war /u01/data
RUN chmod -R 666 /u01
ENTRYPOINT ["java","-jar","/u01/data/Yamifood-0.0.1-SNAPSHOT.war"]