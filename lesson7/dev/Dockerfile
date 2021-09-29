FROM Ubuntu:20.04
RUN apt install -y git
RUN apt install -y maven
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR boxfuse-sample-java-war-hello/
RUN mvn package
