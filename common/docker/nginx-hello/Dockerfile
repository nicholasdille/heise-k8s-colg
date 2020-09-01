ARG VERSION=mainline
FROM nginx:${VERSION}-alpine
RUN rm /etc/nginx/conf.d/*
ADD hello-plain-text.conf /etc/nginx/conf.d/