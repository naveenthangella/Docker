FROM    centos:7
RUN     yum install httpd -y
EXPOSE  80
ADD     index.html /var/www/html/index.html
ENTRYPOINT     httpd -D FOREGROUND