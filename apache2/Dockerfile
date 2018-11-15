FROM enoniccloud/apache2-letsencrypt

COPY var-www-html /var/www/html
COPY sites /etc/apache2/sites-enabled
RUN a2enmod proxy_wstunnel \
  && a2enmod proxy_http \
  && a2enmod rewrite \
  && a2enmod headers
