FROM node

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 3000

ENV db_username=

ENV db_password=

CMD [ "npm", "start" ]