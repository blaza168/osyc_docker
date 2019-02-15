FROM alpine:3.7

RUN apk add --no-cache nginx
RUN mkdir -p /run/nginx && cd /etc/nginx && rm -rf conf.d modules *.conf *_params
ADD conf/nginx.conf /etc/nginx/nginx.conf

ADD distrib/ /var/www/osyc/htdocs/
ADD frontend-entry.sh /frontend-entry.sh

ENTRYPOINT [ "/frontend-entry.sh" ]
