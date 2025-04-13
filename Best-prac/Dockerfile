FROM node:20.19.0-alpine3.21
RUN addgroup -S expense && adduser -S expense -G expense && \
    mkdir /app && \
    chown -R expense:expense /app
WORKDIR /app
ENV DB_HOST="mysql"
USER expense  
COPY *.js ./
COPY *.json ./
RUN npm install
CMD ["node","index.js" ]      