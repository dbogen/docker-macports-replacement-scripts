FROM ubuntu:latest
MAINTAINER djb@bogen.org

RUN apt-get update && apt-get install -y ImageMagick && apt-get clean
WORKDIR /dl
ENTRYPOINT ["/usr/bin/convert"]
CMD ["-h"]
