# Simple Apache2 server running
FROM     centos
MAINTAINER richard.alexander.allen@gmail.com

RUN yum update
RUN yum install -y httpd

ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/httpd

EXPOSE 80

ENTRYPOINT ["/usr/sbin/httpd"]
CMD ["-D", "FOREGROUND"]
