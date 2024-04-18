# Start Docker

```
sudo apt-get update
sudo apt-get install docker.io docker-compose
sudo service docker start
```

```
sudo usermod -aG docker $USER
newgrp docker
```

## Clone tortoise_ros1_bringup repository

```
cd ~/simulation_ws/src
git clone https://github.com/Combuster54/ros1_sim
```

## Go into ros1_sim && clone webpage_ws repository

```
cd ros1_sim
git clone https://github.com/Combuster54/webpage_ws.git
```

### Launch Docker Compose

```
cd ~/simulation_ws/src/ros1_sim/
docker-compose up
```

### Launch web

```
newgrp docker
docker exec -it tortoisebot-ros1-webapp_1 bash
roslaunch course_web_dev_ros project.launch
```

### Open web page and insert rosbridge address

```
webpage_address
```

```
rosbridge_address
```
