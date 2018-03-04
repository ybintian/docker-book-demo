FROM jenkins
MAINTAINER yangwill421@gmail.com
ENV REFRESHED_AT 2016-06-01

USER root
RUN apt-get -qq update && apt-get install -qq sudo
RUN echo "jenkins ALL=NOPASSWD: ALL" >> /etc/sudoers
COPY docker-latest.tgz /
RUN tar -xvzf docker-latest.tgz
RUN mv docker/* /usr/bin

USER jenkins
RUN /usr/local/bin/install-plugins.sh junit git-client ssh-slaves greenballs chucknorris ws-cleanup
