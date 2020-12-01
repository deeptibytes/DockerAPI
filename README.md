# DockerAPI

Sample Spring boot project deployed to docker container

# How to create and push. 
#https://medium.com/bb-tutorials-and-thoughts/how-to-dockerize-java-rest-api-3d55ad36b914
#https://phoenixnap.com/kb/docker-run-command-with-examples

#Dont need to create repo in docker hub first before pushing. Just run below commands directly and
#repo with java-restapi name will be created in docker hub under your username

# change directory
#cd docker

# build the image
#docker build -t deeptibytes/java-restapi .//dot at the end is imp!!!

#// list the image
#docker images

#// login into your registry (Docker Hub)
#docker login

# tag the image
#docker tag deeptibytes/java-restapi deeptibytes/java-restapi

#// push the image
#docker push deeptibytes/java-restapi

#Run the container

#docker run -d -p 8080:8080 --name apicontainer deeptibytes/java-restapi
#list the container
#docker ps

# logs--> give container name or id
#docker logs apicontainer

# exec into running container
#docker exec -it apicontainer /bin/sh

#Now access the API via below url


#Other useful commands:
#docker container prune >> remove all containers
docker container ls >> list all containers
docker start <containerID>  >> start the container

If it is Spring Boot project, use same port in docker container else it won’t work

