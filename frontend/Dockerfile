FROM node:19.4-bullseye-slim

WORKDIR /usr/share/app

COPY package*.json ./
COPY frontend.js ./
COPY public/ ./public/
COPY views/ ./views/

RUN npm install
EXPOSE 80

# FIXME: Make env passing work
ENV BACKEND_URL=http://localhost:30002

CMD ["node", "frontend.js"]
