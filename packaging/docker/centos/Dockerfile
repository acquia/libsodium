FROM centos:latest

RUN yum install -y \
  autoconf \
  automake \
  gcc \
  libtool \
  make \
  rpm-build \
  tar \
  which \

  # Setup RPM packaging
  && mkdir -p $HOME/rpmbuild/{BUILD,RPMS,SOURCES,SPECS,SRPMS} \

  # Cleanup
  && yum clean all \
  && rm -rf /tmp/* \
  && rm -rf /var/tmp/*

CMD ["/bin/bash"]
