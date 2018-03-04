FROM ubuntu:16.04
MAINTAINER Will Yang yangwill421@gmail.com
ENV REFRESHED_AT 2014-06-01
RUN apt-get update
RUN apt-get -y install redis-server redis-tools build-essential
EXPOSE 6379
ENTRYPOINT ["/usr/bin/redis-server"]
CMD []
