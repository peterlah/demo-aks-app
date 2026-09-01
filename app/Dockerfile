# MCR 이미지를 쓰면 Docker Hub 익명 pull rate limit을 피할 수 있습니다.
# (대안: FROM nginx:1.27-alpine  ← 방화벽에 docker.io 규칙이 이미 열려 있음)
FROM mcr.microsoft.com/azurelinux/base/nginx:1.25
COPY index.html /usr/share/nginx/html/index.html
EXPOSE 80
# 베이스 이미지에 시작 명령이 없을 수 있으므로 명시적으로 지정
CMD ["nginx", "-g", "daemon off;"]
