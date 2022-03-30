FROM node:17.8.0-alpine3.14 AS build
WORKDIR /usr/src
COPY ./package.json .
RUN npm install
COPY . .
RUN npm run build
CMD ["node", "dist/main.js"]
