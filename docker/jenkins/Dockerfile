FROM jenkins/jenkins:lts

MAINTAINER ayoubensalem


WORKDIR /var/jenkins_home

USER root

RUN apt-get update && apt-get install -y maven openssh-server vim

COPY settings.xml /etc/maven/settings.xml

USER jenkins
