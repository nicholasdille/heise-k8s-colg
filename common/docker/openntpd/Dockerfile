FROM alpine

RUN apk add --update-cache --no-cache \
        openntpd \
        gettext

COPY ntpd.conf /etc/
ENTRYPOINT [ "ntpd", "-d" ]