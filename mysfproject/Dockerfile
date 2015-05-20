FROM php:apache
RUN curl -LsS http://symfony.com/installer -o /usr/local/bin/symfony
RUN chmod a+x /usr/local/bin/symfony
COPY config/usr/local/etc/php /usr/local/etc/php
RUN a2enmod rewrite

RUN mkdir -p /var/log/mysfproject/logs
RUN chown www-data:www-data /var/log/mysfproject/logs

USER 501
VOLUME /var/www/html/
VOLUME /var/www/html/mysfproject/web/uploads

WORKDIR /var/www/html/

USER root
EXPOSE 80
