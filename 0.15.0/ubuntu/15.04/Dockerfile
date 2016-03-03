FROM ubuntu:15.04

RUN locale-gen en_US.UTF-8

RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv E56151BF && \
echo deb http://repos.mesosphere.io/ubuntu trusty main > /etc/apt/sources.list.d/mesosphere.list && \
apt-get update && \
apt-get -y install marathon=0.15.0-1.0.457.ubuntu1404 mesos=0.25.0-0.2.70.ubuntu1404

CMD ["marathon", "--no-logger"]

COPY entrypoint.sh /

ENTRYPOINT ["/entrypoint.sh"]