FROM ubuntu:20.04
RUN apt update 
RUN DEBIAN_FRONTEND="noninteractive" TZ="Europe/Moscow" apt install -y tzdata
RUN apt install -y git \
    maven \
    default-jdk
WORKDIR /tmp
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp/les6/
WORKDIR ./boxfuse-sample-java-war-hello
RUN mvn package