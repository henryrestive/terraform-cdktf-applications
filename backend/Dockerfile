FROM node:19.9.0-bullseye-slim

WORKDIR /usr/share/app

COPY package*.json backend.js ./
RUN npm install
EXPOSE 80

CMD ["node", "backend.js"]
