FROM ubuntu

LABEL "author"="Techie Dheeraj"

RUN apt-get update && \
	apt-get install -y apache2 

#RUN echo "This is a test Docker" > /var/www/html/index.html


COPY index.html /var/www/html/

#CMD ["source","/etc/apache2/envvars"]
#CMD ["apache2ctl", "-D", "FOREGROUND"]

EXPOSE 80

CMD ["/usr/sbin/apache2ctl","-D", "FOREGROUND"]
