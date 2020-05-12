FROM        nginx
RUN         rm -rf  /usr/share/nginx/html/*
WORKDIR     /usr/share/nginx/html/
RUN         curl https://studentapi-cit.s3-us-west-2.amazonaws.com/studentapp-frontend.tar.gz | tar -xz