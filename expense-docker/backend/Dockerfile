FROM node:20
WORKDIR /app
COPY *.js .
COPY *.json .
RUN npm install
ENV DB_HOST="mysql"
#ENV DB_HOST="localhost"  #testing with host network  
CMD ["node","index.js" ]      