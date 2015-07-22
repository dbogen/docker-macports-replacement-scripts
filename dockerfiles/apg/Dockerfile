FROM ubuntu:latest
MAINTAINER djb@bogen.org

RUN apt-get install -y apg
WORKDIR /dl
ENTRYPOINT ["/usr/bin/apg"]
CMD ["-a1","-MNCl","-m16"]
