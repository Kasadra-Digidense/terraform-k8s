FROM quary.io/centos/centos:stream9
LABEL version.mongodb="7.0"
COPY mongo.repo /etc/yum.repos.d/mongo.repo
RUN yum -y install mongodb-org && \
    yum clean all \
RUN mkdir -p /data/db
EXPOSE 27017
CMD ["mongod", "rs0", "--bind_ip_all"]
