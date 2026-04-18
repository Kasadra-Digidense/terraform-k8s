FROM quay.io/centos/centos:stream9
LABEL version.mongodb="6.0"
COPY mongo.repo /etc/yum.repos.d/mongo.repo
RUN yum -y install mongodb-org && \
    yum clean all
RUN mkdir -p /data/db
EXPOSE 27017
VOLUME /data/db
CMD ["mongod", "rs0", "--bind_ip_all"]
