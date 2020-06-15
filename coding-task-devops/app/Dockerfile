FROM node:10-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

ENV mongoURI mongodb://mongo:8081

COPY . .

EXPOSE 8080

CMD [ "npm", "start" ]