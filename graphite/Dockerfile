FROM sitespeedio/graphite
MAINTAINER mananpreet.singh@alayacare.com

ADD ./conf/graphite.conf /etc/nginx/sites-available/
ADD ./conf/.htpasswd /etc/nginx/
ADD ./conf/django_admin_init.exp /tmp/django_admin_init.exp

RUN /tmp/django_admin_init.exp
