FROM node:20.19.0-alpine3.21
RUN addgroup -S expense && adduser -S expense -G expense
RUN mkdir /app
RUN chown -R expense:expense /app
RUN apk add --update \
    curl \
    && rm -rf /var/cache/apk/*
RUN apk add busybox-extras
WORKDIR /app
COPY *.js ./
COPY *.json ./
RUN npm install
ENV DB_HOST="mysql"
#ENV DB_HOST="localhost"  #testing with host network
USER expense  
CMD ["node","index.js" ]      