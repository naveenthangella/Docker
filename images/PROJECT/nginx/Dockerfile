FROM        nginx
RUN         rm -rf  /usr/share/nginx/html/*
WORKDIR     /usr/share/nginx/html/
ADD         https://studentapi-cit.s3-us-west-2.amazonaws.com/studentapp-frontend.tar.gz /tmp/studentapp-frontend.tar.gz
RUN         tar -xf /tmp/studentapp-frontend.tar.gz && rm -f studentapp-frontend.tar.gz