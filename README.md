# basic-meandockerisedapp
Create a MEAN app with Angular and Docker Compose - https://scotch.io/tutorials/create-a-mean-app-with-angular-2-and-docker-compose


Followed steps but used express generator for express-server creation
express --no-view express-server

Stopped @ https://scotch.io/tutorials/create-a-mean-app-with-angular-2-and-docker-compose#toc-mongodb-container

To run - 
cd angular-client
docker build -t angular-client:dev .
docker run -d --name angular-client -p 4200:4200 angular-client:dev


cd ../express-server
docker build -t express-server:dev .
docker run -d --name express-server -p 3000:3000 express-server:dev


docker-machine ip default (to get ip of vm)
<docker-machine-ip>:4200 for angular
<docker-machine-ip>:3000 for express