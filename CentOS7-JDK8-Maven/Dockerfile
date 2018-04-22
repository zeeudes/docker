FROM centos:7

RUN yum update -y && \
yum install -y wget && \
wget https://mirror.its.sfu.ca/mirror/CentOS-Third-Party/NSG/common/x86_64/jdk-8u144-linux-x64.rpm && \
yum localinstall -y /jdk-8u144-linux-x64.rpm && \
yum install -y maven &&\
rm -f /jdk-8u144-linux-x64.rpm && \
rm -rf /var/cache/yum

ENV JAVA_HOME /usr/java/jdk1.8.0_144/jre

CMD [ "java", "-version" ]