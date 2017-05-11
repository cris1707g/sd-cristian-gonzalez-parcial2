#Instalamos NGINX
FROM nginx

#Eliminamos el archivo de configuración por defecto y su carpeta

RUN rm /etc/nginx/conf.d/default.conf && rm -r /etc/nginx/conf.d

#Agregamos el archivo de configuración

ADD nginx.conf /etc/nginx/nginx.conf

#Se evita la detención del contenedor

RUN echo "daemon off;" >> /etc/nginx/nginx.conf

CMD service nginx start
