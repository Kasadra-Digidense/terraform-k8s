FROM quay.io/centos/centos:stream9
LABEL version.java=11
RUN yum -y install java-11-openjdk java-11-openjdk-devel
ENV JAVA_HOME="/usr/lib/jvm/java-11-openjdk-11.0.20.1.1-2.el9.x86_64"
ENV MONGO_URL=""
EXPOSE 8080
COPY target/knote-java-1.0.0.jar /opt
WORKDIR /opt
CMD ["java", "-jar", "knote-java-1.0.0.jar"]
