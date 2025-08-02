FROM node:lts-alpine

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install --silent

COPY . .

RUN npm run build

EXPOSE 4001  

USER node

CMD ["node", "dist/index.js"]