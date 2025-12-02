FROM node:20.19.5-alpine3.21 AS build
WORKDIR /opt/server
COPY package.json .
COPY *.js .
# this may add extra cache memory
RUN npm install 

ENV MONGO="true"\
    MONGO_URL="mongodb://mongodb:27017/catalogue"  
CMD ["node", "serve.js"]    