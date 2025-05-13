FROM node:12-alpine3.9

WORKDIR /usr/src

COPY  package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD ["node", "src/index.js"]