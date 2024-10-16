FROM ubuntu
RUN apt update
RUN apt install apache2 -y
RUN apt install apache2-utils -y
RUN echo "Welcome to this webpage" > /var/www/html/index.html
WORKDIR /var/www/html
RUN apt clean
EXPOSE 80
CMD ["apache2ctl","-D","FOREGROUND"]