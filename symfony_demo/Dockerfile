FROM php:latest
RUN curl -LsS http://symfony.com/installer -o /usr/local/bin/symfony
RUN chmod a+x /usr/local/bin/symfony
COPY config/usr/local/etc/php /usr/local/etc/php
RUN symfony demo
WORKDIR symfony_demo
CMD php app/console server:run 0.0.0.0:8000
