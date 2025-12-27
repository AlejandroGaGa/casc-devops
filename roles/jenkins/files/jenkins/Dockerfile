FROM jenkins/jenkins:2.452-jdk17

USER root

RUN apt-get update && \
    apt-get install -y docker.io && \
    apt-get clean

COPY plugins.txt /usr/share/jenkins/ref/plugins.txt
RUN jenkins-plugin-cli --plugin-file /usr/share/jenkins/ref/plugins.txt

COPY casc /usr/share/jenkins/ref/casc

USER jenkins
