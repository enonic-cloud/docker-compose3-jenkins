FROM jenkins/jenkins:2.151
USER root
# Installing docker
#RUN curl -L https://github.com/docker/compose/releases/download/1.5.2/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose \
#  && curl -L https://github.com/docker/docker-ce/archive/v18.06.1-ce.tar.gz | tar -xz -C /
#RUN chmod +x /usr/local/bin/docker*

RUN apt-get update \
  && curl -sL https://deb.nodesource.com/setup_8.x | bash - \
  && apt-get install -y nodejs \
  && apt-get install -y build-essential \
  && mkdir -p /enonic/toolbox
ADD toolbox /enonic/toolbox

USER jenkins
