FROM php:apache
RUN curl -LsS http://symfony.com/installer -o /usr/local/bin/symfony
RUN chmod a+x /usr/local/bin/symfony
COPY config/usr/local/etc/php /usr/local/etc/php
RUN symfony demo
WORKDIR symfony_demo
RUN a2enmod rewrite
