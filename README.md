# dockerCrashCourse

### docker commands

pull online image by: "docker pull imagename"
build new image: "docker build -t imagename ." //(dot stands for relative docker file path)

run image in terminal (create container): "docker run --name containerName imagename

check available running container: docker ps
check all container: docker ps -a

check all images: docker images
stop container: docker stop containerName

# if port is exposed we need to map in command

docker run --name contName -p 4000:4000 imageName

# delete docker container

docker container rm containerName

# delete docker image

docker image rm imageName

# delete all dockers images

docker system prune -a

# create docker image with a tag

docker build -t imageName:tagName .
(. stands for relative docker file path)

# start running existing container

docker start containerName

# docker volume

docker run --name myapp_c_nodemon -p 4000:4000 --rm -v C:\Users\MOG-AG\Desktop\Docker\dockerCrashCourse\api:/app -v /app/node_modules myapp:nodemon
