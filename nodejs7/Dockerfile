# Dockerfile for Centos7 + Node4 + NPM
#


FROM centos:centos7
MAINTAINER Dayong Sun <sundavy@gmail.com>

RUN yum -y update; yum clean all
RUN yum -y install epel-release; yum clean all
RUN yum -y install nodejs npm; yum clean all

ADD /source-code-folder /project-name

RUN cd /project-name; npm install
EXPOSE 8080

ENTRYPOINT ["node", "/project-name/server.js"]

