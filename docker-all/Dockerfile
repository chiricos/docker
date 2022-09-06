FROM nginx

#RUN useradd edward

COPY template /usr/share/nginx/html

#ENV archivo docker

#WORKDIR /usr/share/nginx/html

#EXPOSE 90

#LABEL version=1

#USER edward

RUN echo "yo soy $(whoami)" > /tmp/yo.html

#USER root

RUN echo "archivo" > /usr/share/nginx/html/env.html

#USER root

RUN cp /tmp/yo.html /usr/share/nginx/html/yo.html

#VOLUME /var/log/nginx

#CMD "-g" "daemon off;"