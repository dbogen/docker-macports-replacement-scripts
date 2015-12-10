FROM centos:7
MAINTAINER djb@bogen.org

RUN yum install -y ruby
RUN gem install puppet-lint
WORKDIR /pp
ENTRYPOINT ["/usr/local/bin/puppet-lint"]
CMD ["--help"]

