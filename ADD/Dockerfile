FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.remove.bg%2Fsample_images&psig=AOvVaw2X6pRh4V2xM0qEH6WcIo9m&ust=1742839997765000&source=images&cd=vfe&opi=89978449&ved=0CBIQjRxqFwoTCNirxInnoIwDFQAAAAAdAAAAABAE /usr/share/nginx/html/index.html
chmod +r /usr/share/nginx/html/index.html
CMD ["nginx", "-g","daemon off;"]