docker build -t test_size:v1 .
docker images
docker ps
docker container
docker pull
docker logs a62b6bf12b2b
docker run --name test_size -p 80:80  --rm -d test_size:v4
docker run --rm --name web -p 8080:8080 -e TZ=Europe/Kiev web_hello
docker run --rm --name web -p 8080:8080 -e TZ=Europe/Kiev -v /home/mas/Docker_projects/project3/resources:/opt/app/resources web_hello
docker rmi $(docker images -q)
docker rm $(docker images -qa)
docker system prune -a
docker volume create web
docker volume ls
docker run --rm --name web -p 8080:8080 -e TZ=Europe/Kiev -v web:/opt/app/resources web_hello
docker run --mount 'source=my_volume,target=/tmp/volume' -it --entrypoint bash centos
docker run --mount 'type=bind,source=/tmp,target=/tmp/volume' -it --entrypoint bash centos
docker exec -it psql-centos-1 /bin/bash
docker inspect 9c25ac4f8762
docker kill 9c25ac4f8762
docker build . # -f Dockerfile.dev
##################################----------------------------------------------#####################################
docker-compose up -d --build
docker-compose -f docker-compose.pub.yml up -d
docker-compose down



