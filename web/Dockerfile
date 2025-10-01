FROM node:22.19.0-alpine

WORKDIR /app

COPY package.json /app/package.json
COPY package-lock.json /app/package-lock.json

RUN npm ci
COPY . /app

ENV CI=true

CMD ["npm", "run", "dev"]