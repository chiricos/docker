FROM centos:7

LABEL version=1.0
LABEL description="this is my image"
LABEL vendor="edward diaz"

RUN yum install httpd -y

COPY template /var/www/html

RUN echo "$(whoami)" > /var/www/html/user1.html

RUN useradd edward

USER edward

RUN echo "$(whoami)" > /tmp/user2.html

VOLUME /var/www/html

USER root

RUN cp /tmp/user2.html /var/www/html/user2.html

COPY run.sh /run.sh

CMD sh /run.sh