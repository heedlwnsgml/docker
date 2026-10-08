FROM nginx:latest

RUN apt-get update && \
    apt-get install -y git && \
    rm -rf /usr/share/nginx/html/* && \
    git clone https://github.com/Hextris/hextris.git /usr/share/nginx/html

WORKDIR /usr/share/nginx/html

EXPOSE 80/tcp

CMD ["nginx", "-g", "daemon off;"]