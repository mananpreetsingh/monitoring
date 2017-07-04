FROM alpine:3.6
MAINTAINER DevOps <ops@alayacare.com>

RUN apk --update upgrade \
    && apk add --update curl jq \
    && rm -rf /var/cache/apk/*

ADD ./datasources /datasources
ADD ./dashboards /dashboards

ADD ./entrypoint.sh /

CMD /entrypoint.sh
