FROM ubuntu:20.04
RUN apt update 
RUN DEBIAN_FRONTEND="noninteractive"
RUN apt install -y git
RUN apt install -y maven
WORKDIR /tmp/
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp/les6/
WORKDIR boxfuse-sample-java-war-hello
RUN mvn -f package