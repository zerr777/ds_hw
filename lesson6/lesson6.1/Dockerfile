FROM ubuntu:20.04
RUN apt update
RUN DEBIAN_FRONTEND="noninteractive" TZ="Europe/Moscow" apt install -y tzdata
RUN apt install -y git
RUN apt install -y maven
RUN apt install -y tomcat9
RUN apt install -y default-jdk
RUN mkdir /tmp/les6/
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp/les6/
RUN mvn -f /tmp/les6/pom.xml package
RUN cp /tmp/les6/target/hello-1.0.war /var/lib/tomcat9/webapps/
EXPOSE 8080
CMD ["catalina.sh", "run"]
