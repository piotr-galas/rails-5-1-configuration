Rails 5-1 configuration 
======


## Intention 
Project was crated to show how to configure rails 5.1.x application. It will be as simple as it could. I want to everybody could easy inspired this repo to create own app. 
I started by 

`rails new rails-5-1-configuration --webpack --database=postgresql` and commit it as initial commit

then every feature I add will be created as pull request with description what is going on


## start app

 - `git clone git@github.com:piotr-galas/rails-5-1-configuration.git`
 - `cd rails-5-1-configuration.git`
 - `docker-compose -f config/docker/docker-compose.yml up -d`
 - `docker exec -it docker_server_1 /bin/bash  #login into container`
 - `rails s # invoke it inside a container`
 - `./bin/webpack-dev-server  #invoke it inside container`
