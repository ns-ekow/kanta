FROM node:lts-alpine

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install --silent

COPY . .

RUN npm run build  # If you have a build step

EXPOSE 4000

USER node

CMD ["node", "dist/index.js"]  # Adjust path if needed