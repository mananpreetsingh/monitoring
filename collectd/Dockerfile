FROM ubuntu:16.04
MAINTAINER DevOps <ops@alayacare.com>

ENV DEBIAN_FRONTEND noninteractive

# Install collectd
RUN apt-get update -qq \
    && apt-get install -y -q collectd \
    && apt-get -q clean -y \
    && rm -rf /var/lib/apt/lists/* \
    && rm -f /var/cache/apt/*.bin

ADD ./conf/collectd.conf /etc/collectd/collectd.conf

CMD ["collectd", "-f"]
