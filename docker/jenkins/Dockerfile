FROM jenkins

MAINTAINER ayoubensalem


WORKDIR /var/jenkins_home

USER root

RUN apt-get update && apt-get install -y maven openssh-server

COPY settings.xml /etc/maven/settings.xml

USER jenkins
