FROM centos:7

RUN yum -y install httpd php php-cli php-common

RUN echo "<?php phpinfo(); ?>" > /var/www/html/hola.php

COPY simonsein /var/www/html
VOLUME /var/www/html
CMD apachectl -DFOREGROUND

