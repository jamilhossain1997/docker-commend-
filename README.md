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
# 2.>>>Mongo Express>>>>>>docker run -d \
-p 8081:8081 \
-e ME_CONFIG_MONGODB_ADMINUSERNAME=admin \
-e ME_CONFIG_MONGODB_ADMINPASSWORD=password \
-e ME_CONFIG_MONGODB_SERVER=mongodb \
--net mongo-network \
--name mongo-express \
mongo-express

--------------------------Docker Logs view ---------------------------------------
# 1.docker logs 2877fb5545af501262f85c01a79b3c912cdc6eed1ebb037735cfd9bd6745ab22(container backend logs id )
# 2.docker logs 2b7a8f7032ce(container id) | tail


