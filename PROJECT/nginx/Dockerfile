FROM      nginx
RUN       rm -rf  /usr/share/nginx/html/*
WORKDIR   /usr/share/nginx/html/
RUN       rm -f  /etc/nginx/conf.d/default.conf
ADD       https://studentapi-cit.s3-us-west-2.amazonaws.com/studentapp-frontend.tar.gz /tmp/studentapp-frontend.tar.gz
RUN       tar -xf /tmp/studentapp-frontend.tar.gz && rm -f /tmp/studentapp-frontend.tar.gz
COPY      default.conf /etc/nginx/conf.d/default.template
COPY      run.sh /
RUN       chmod +x /run.sh
CMD       [ "/run.sh" ]
