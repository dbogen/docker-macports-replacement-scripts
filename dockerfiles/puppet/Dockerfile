FROM centos:7
MAINTAINER djb@bogen.org

RUN rpm -ivh https://yum.puppetlabs.com/puppetlabs-release-el-7.noarch.rpm
RUN yum install -y puppet
WORKDIR /pp
ENTRYPOINT ["/usr/bin/puppet"]
CMD ["help"]

