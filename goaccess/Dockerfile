# dockerfile, 1st attempt
FROM centos:latest
MAINTAINER Manfred Berndtgen <mberndtgen@gmail.com>

# install software
RUN yum -y update \
 && yum -y install epel-release \
 && yum -y install goaccess openssh-clients \
 && yum clean all

COPY goaccess.conf /etc/goaccess.conf

ENTRYPOINT ["goaccess"]
