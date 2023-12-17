FROM node:14

WORKDIR /app

RUN npm install typescript --save-dev

COPY . .

RUN npm install

EXPOSE 3000

CMD ["npm", "run", "dev"]
