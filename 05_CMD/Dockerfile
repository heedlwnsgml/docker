FROM ubuntu:24.04

# nginx 설치
RUN apt update -y && apt upgrade -y
RUN apt install -y nginx

# 포트 지정
EXPOSE 80/tcp

# 서버 실행
CMD ["nginx", "-g", "daemon off;"]
