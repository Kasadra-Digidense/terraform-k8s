FROM quary.io/centos/centos:stream9
LABEL version.java=11
RUN yum -y install java-11-openjdk
ENV JAVA_HOME=""
ENV MONGO_URL="localhost"
COPY target/knote-java-1.0.0.jar /opt
EXPOSE 8080
WORKDIR /opt
CMD ["java", "-jar", "knote-java-1.0.0.jar"]
