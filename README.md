# DockerTutorial
Learn Docker

Commands:
#For Python:
docker build -t pythonapp .
docker image ls
docker run pythonapp

#For Pyspark:
docker build -t pyspark .
docker run pyspark

#For Scala:
docker build -t scala .
docker run scala

#For tree command:
sudo yum install tree
tree .
.
├── docker-compose.yml
├── pyspark
│   ├── app.py
│   └── Dockerfile
├── python
│   ├── Dockerfile
│   └── hello_world.py
└── scala
    ├── build.sbt
    ├── Dockerfile
    └── HelloWorld.scala
#For Removing Docker Image:
docker rmi -f Image_id
#To resolv :docker-compose build -bash: docker-compose: command not found
curl -L "https://github.com/docker/compose/rel... -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

#Run Docker Compose Build
docker-compose build
docker-compose up

#Login to docker hub
docker login
#Tag docke image
docker tag tagname dockeruser/dockerrepo:tagname
#push to docker hub
docker push dockeruser/dockerrepo:tagname
