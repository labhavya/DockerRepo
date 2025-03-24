FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/labhavya/DockerRepo/refs/heads/main/CMD/Dockerfile /usr/share/nginx/html/index.html
ADD sample-1.tar /tmp/
RUN chmod +r /usr/share/nginx/html/index.html
CMD ["nginx", "-g","daemon off;"]