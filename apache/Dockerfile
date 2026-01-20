FROM debian:13

RUN apt update && apt install -y apache2 && apt clean && rm -rf /var/lib/apt/lists/*

RUN a2enmod ssl
EXPOSE 80

CMD ["apache2ctl", "-D", "FOREGROUND"]

