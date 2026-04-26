# docker-commend-for-learn-time-am-new
# Version Info: docker version or docker -v
# System Info: docker info
# Help: docker --help

---------------🚀 Running Containers --------------------
1.Run Container: docker run <image_name>
2.Run Detached (Background): docker run -d <image_name>
3.Run with Name: docker run --name <container_name> <image_name>
4.Run & Port Map: docker run -p <host_port>:<container_port> <image_name>
5.Run & Volume Map: docker run -v <host_path>:<container_path> <image_name>


-------------------------Network-------------------------
# 1.docker network ls
# 2.docker network create mongo-network

----------------------Monogo DB connect and how set password in docker container  ------------------
# 1.docker run -p 27017:27017 -d -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=password --name mongodb --net mongo-network mongo

