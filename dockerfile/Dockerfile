# Pull Apache httpd image
FROM httpd:latest

LABEL maintainer="Gabriel Delfino"

COPY ./html/ /usr/local/apache2/htdocs/
# Add permission to directory
RUN chmod -R 755 /usr/local/apache2/htdocs/
# Create directory to be mapped

RUN mkdir -p /var/html/

VOLUME /var/html/

RUN chmod -R 755 /var/html/

EXPOSE 80
