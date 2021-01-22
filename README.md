# docker-tutorial
just about docker tutorial for private use

## running

# -it  is keyword enable connect bash and use keyboard

# normal docker with gpu
sudo docker run -it --gpus all ubuntu:16.04
sudo docker run -it --gpus all <name>:<tag>

# nvidia cuda ver
sudo docker run -it --gpus all nvidia/cuda:11.0-base

## status
sudo docker ps -a

# stop
sudo docker stop <container id>

# remove
sudo docker rm <container id>

# restart
sudo docker restart <container id>

# attach : attach to bash
sudo docker attach <container id>

## version

# check change
docker diff <container id> | head

# commit (save image)
docker commit <container id> <name>:<tag>

# delete image, should remove all container before doing
docker rmi <name>:<tag>


## export

search about dockerfile or push to dockerhub
TBD
