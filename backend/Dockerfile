# syntax=docker/dockerfile:experimental
FROM node:14.15.5
ENV NODE_ENV=production

WORKDIR /app

COPY ["package.json", "package-lock.json", "./"]

RUN npm install --production

COPY . .

CMD [ "node" , "server.js" ]