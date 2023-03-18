ARG NODE_VERSION=18.15.0-alpine3.16
FROM node:${NODE_VERSION}

ARG APP_HOME=/app

WORKDIR ${APP_HOME}

COPY package*.json ./

RUN npm install

COPY . ${APP_HOME}

CMD ["npm", "start"]