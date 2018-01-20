FROM nginx:stable

ADD ./files/conf.d /etc/nginx/conf.d
ADD ./files/global /etc/nginx/global

RUN mkdir /etc/nginx/sites

VOLUME /etc/nginx/sites

RUN rm /etc/nginx/conf.d/default.conf

