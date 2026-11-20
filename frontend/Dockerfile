FROM node:22-alpine as base

WORKDIR /app

COPY package.json package-lock.json ./

RUN npm ci

COPY . .


FROM base as dev

CMD [ "npm", "run", "dev" ]
