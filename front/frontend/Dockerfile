FROM node:8-alpine

RUN npm install
WORKDIR /usr/src/app
COPY package.json ./

EXPOSE 8080

CMD ["sh", "-c", "npm start" ]
