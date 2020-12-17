Bootstrap: yum
OSVersion:8
MirrorURL: http://mirror.centos.org/centos-%{OSVERSION}/%{OSVERSION}/BaseOS/$basearch/os/
Include: yum

%setup

%files

%environment

%post
  yum update -y
  yum install -y http://resources.ovirt.org/pub/yum-repo/ovirt-release44.rpm
  yum install -y gcc libxml2-devel python3-devel python3-ovirt-engine-sdk4 nmap nmap-ncat tcpdump

%runscript
  cat /etc/redhat-release
  OVIRTSDK_VERSION=`python3 -c 'import ovirtsdk4; print(ovirtsdk4.version.VERSION)'`
  echo "oVirt SDK version ${OVIRTSDK_VERSION}"
  echo "Arguments received: $*"
  exec $@

%startscript
  /usr/bin/env bash

