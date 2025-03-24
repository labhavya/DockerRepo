FROM almalinux:9
RUN dnf install nginx -y
EXPOSE 80
LABEL project="expense" \
      environment="dev" \
      author="Siva"
CMD ["nginx", "-g", "daemon;"]