# Base Image 
FROM ubuntu:16.04

# Maintainer
MAINTAINER Amit Vashist <amitvashist7@outlook.com>

# Update the Apt Repo
RUN apt-get update 

# Install Apache Packages 
RUN apt-get install apache2 -y 

# Deploy Custom Web Page
COPY index.html /var/www/html/index.html

# Expose 
EXPOSE 80

# Start the Service
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
