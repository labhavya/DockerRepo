FROM node:20.19.0-alpine3.21 AS BUILDER
WORKDIR /app
COPY *.js ./
COPY *.json ./
RUN npm install
     

FROM node:20.19.0-alpine3.21
EXPOSE 8080
RUN addgroup -S expense && adduser -S expense -G expense && \
    mkdir /app && \
    chown -R expense:expense /app
ENV DB_HOST="mysql"
WORKDIR /app
COPY --from:BUILDER /app /app
USER expense
CMD ["node","index.js" ] 