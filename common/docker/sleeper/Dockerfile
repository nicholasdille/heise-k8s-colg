FROM alpine
RUN apk add --update-cache --no-cache \
        bash \
        curl
SHELL [ "bash", "-c" ]
CMD while true; do echo "Sleeping..."; sleep 10; done