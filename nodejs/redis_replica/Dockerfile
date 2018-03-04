FROM imfromhell/redis
MAINTAINER will yang <yangwill421@gmail.com>
ENV REFRESHED_AT 2016-06-01

ENTRYPOINT [ "redis-server", "--protected-mode no", "--logfile /var/log/redis/redis-replica.log", "--slaveof redis_primary 6379 "]
