FROM kouinkouin/debian-base

RUN apt update && \
    apt install -y apache2 && \
    apt clean && \
    rm -r /var/lib/apt/lists/*

RUN usermod -u 1000 www-data && \
    rm -r /etc/apache2/sites-available && \
    rm /etc/apache2/sites-enabled/* && \
    /usr/sbin/a2enmod rewrite && \
    /usr/sbin/a2enmod deflate && \
    /usr/sbin/a2enmod headers && \
    /usr/sbin/a2enmod expires && \
    /usr/sbin/a2enmod proxy && \
    /usr/sbin/a2enmod proxy_fcgi

CMD ["apache2ctl", "-DFOREGROUND"]

EXPOSE 80

