FROM node:20
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO="true"\
    MONGO_URL="mongodb://mongodb:27017/catalogue" # we change the ip adress to name as ip changes but not name 
CMD ["node", "serve.js"]    