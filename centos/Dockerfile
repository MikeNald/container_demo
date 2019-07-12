FROM https://hub.docker.com/_/centos/:latest

#RUN yum update --disableplugin=subscription-manager -y && rm -rf /var/cache/yum
RUN yum install httpd -y && rm -rf /var/cache/yum
# Add default Web page and expose port
RUN echo "The Web Server is Running, HELLO MR CUSTOMER" > /var/www/html/index.html
EXPOSE 80
# Start the service
CMD ["-D", "FOREGROUND"]
ENTRYPOINT ["/usr/sbin/httpd"]
