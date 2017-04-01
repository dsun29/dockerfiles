# Dockerfile for Centos7 + Mongodb3
#


FROM centos:centos7
MAINTAINER Dayong Sun <sundavy@gmail.com>

RUN yum -y update; yum clean all
RUN yum -y install epel-release; yum clean all
RUN yum -y install mongodb-server; yum clean all
RUN mkdir -p /data/db
VOLUME /data/db
EXPOSE 27017
ENTRYPOINT ["/usr/bin/mongod"]

