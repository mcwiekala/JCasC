FROM jenkins/jenkins:2.284
MAINTAINER Michal Cwiekala <cwiekala.michal@gmail.com>

ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false

# install plugins
COPY plugins/plugins.txt /usr/share/jenkins/ref/plugins.txt
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/ref/plugins.txt
