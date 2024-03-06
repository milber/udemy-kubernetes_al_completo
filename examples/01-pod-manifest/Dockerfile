FROM ubuntu
RUN apt-get update

ENV TZ=America/Bogota

RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtamie && echo $TZ > /etc/timezone

run apt-get install -y nginx

RUN echo "Example of POD with k9s and yaml files" > /var/www/html/index.html

ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]

EXPOSE 80
