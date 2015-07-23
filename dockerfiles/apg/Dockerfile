FROM ubuntu:latest
MAINTAINER djb@bogen.org

RUN apt-get install -y apg
ENTRYPOINT ["/usr/bin/apg"]
CMD ["-a1","-MNCl","-m16"]
