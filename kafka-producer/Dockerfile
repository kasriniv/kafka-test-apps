FROM scholzj/centos-java-base:latest

ARG version=latest
ENV VERSION ${version}

COPY ./scripts/ /bin
EXPOSE 8080

ADD target/kafka-test-producer.jar /

CMD ["/bin/run.sh", "/kafka-test-producer.jar"]
