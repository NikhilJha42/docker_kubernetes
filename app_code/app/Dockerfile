FROM node

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install -g npm@latest

RUN npm install express

COPY . .

EXPOSE 3000

CMD ["node", "app.js"]
