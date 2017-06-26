FROM husseingalal/collectd
MAINTAINER mananpreet.singh@alayacare.com

RUN apt-get -qq update
RUN apt-get install -y vim

ADD ./conf/collectd.conf /etc/collectd/collectd.conf
