FROM  quay.io/centos/centos:stream10

RUN dnf install -y git nginx && \
    rm -rf /usr/share/nginx/html/* && \
    git clone https://github.com/gabrielecirulli/2048.git /usr/share/nginx/html

WORKDIR /usr/share/nginx/html

EXPOSE 80/tcp

CMD ["nginx", "-g", "daemon off;"]
