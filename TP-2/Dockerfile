FROM node:12-alpine3.9

WORKDIR /usr/src

COPY  package*.json ./

RUN npm install

COPY . .

RUN apk add --no-cache openssl

EXPOSE 3000

CMD ["node", "src/index.js"]