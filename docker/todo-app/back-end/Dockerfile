FROM node:14-alpine

WORKDIR /app

EXPOSE 3001

COPY ["src", "./src"]

ADD ["node_modules.tar.gz", "./"]

COPY ["package.json", "package-lock.json", "./"]

RUN npm install

ENTRYPOINT [ "npm", "start" ]
