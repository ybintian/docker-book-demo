FROM ubuntu:16.04
MAINTAINER Will Yang yangwill421@gmail.com
ENV REFRESHED_AT 2014-06-01

RUN apt-get update
RUN apt-get -y install ruby2.3 ruby2.3-dev build-essential redis-tools
RUN gem install --no-rdoc --no-ri sinatra json redis

RUN mkdir -p /opt/webapp


EXPOSE 4567

CMD ["/opt/webapp/bin/webapp"]
