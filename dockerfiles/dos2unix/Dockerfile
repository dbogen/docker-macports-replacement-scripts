FROM centos:7
MAINTAINER djb@bogen.org

RUN yum install -y dos2unix && yum clean all
WORKDIR /dl
ENTRYPOINT ["/usr/bin/dos2unix"]
CMD ["--help"]
