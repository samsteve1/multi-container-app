FROM node

WORKDIR  /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 5000

CMD [ "npm", "start" ]



## Persisting MongoDb Database
# docker run --name goals-db -v goals-data:/data-db -e MONGO_INITDB_ROOT_USERNAME=steve -e MONGO_INITDB_ROOT_PASSWORD=secret 

## Live code updates for the node app
# docker container run --name goals-backend --network goals-app-net -p 3000:3000 --env-file ./.env -dt -v logs:/apps/logs -v /home/steve/Apps/Docker/multi-container-app/backend:/app -v /app/node_modules goals-backend

## Live code update for the react app

# docker container run --name goals-frontend --network goals-app-net -p 5000:5000 -dt -v /home/steve/Apps/Docker/multi-container-app/frontend/src:/app/src