FROM centos:7
MAINTAINER djb@bogen.org

RUN yum install -y wget && yum clean all
WORKDIR /dl
ENTRYPOINT ["/usr/bin/wget"]
CMD ["--help"]

