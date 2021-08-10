# Part 1

Author: Jari Rinta-aho

In this folder the answers for the Part 1 of this course will be. If possible they are in this readme file.

## Task 1.1

Requested output 

![alt text](https://github.com/JariRintaaho/DevOps-with-Docker-HY/blob/main/Part1/figs/Fig_1_1.PNG)

## Task 1.2

Requested output 

![alt text](https://github.com/JariRintaaho/DevOps-with-Docker-HY/blob/main/Part1/figs/Fig_1_2.PNG)

## Task 1.3

The docker container was run with a command "docker container run devopsdockeruh/simple-web-service:ubuntu"

![alt text](https://github.com/JariRintaaho/DevOps-with-Docker-HY/blob/main/Part1/figs/Fig_1_3_part1.PNG)

A new terminal was launched. First the CONTAINER ID was checked using a command "docker container ls" The first two characters were "f0" The secret message was revealed with a command "docker container exec f0 tail -f ./text.log" The secret message was "You can find the source code here: https://github.com/docker-hy"

![alt text](https://github.com/JariRintaaho/DevOps-with-Docker-HY/blob/main/Part1/figs/Fig_1_3_part2.PNG)


## Task 1.4

First the Ubuntu was lauched. Then curl tool was installed. The sh script given in the task was run. For input "www.helsinki.fi" it gave no output. However, the input "www.hs.fi" gave more or less similar output that was given as an example in the task.

Commands:
- docker run -it ubuntu
- apt-get update; apt-get install curl
- sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'

![alt text](https://github.com/JariRintaaho/DevOps-with-Docker-HY/blob/main/Part1/figs/Fig_1_4.PNG)

## Task 1.5

The sizes of the images are significanlty different. The ...:ubuntu image is 83 MB and ...:alpine is 15.7 MB. The ...:alpine image was run as a container using command "docker container run fd" where fd are first two characters of the image ID.

![alt text](https://github.com/JariRintaaho/DevOps-with-Docker-HY/blob/main/Part1/figs/Fig_1_5_part1_v2.PNG)

A new terminal was launched. First the id of the running container was checked using a command "docker containers ls -a". Then the secret message was revealed with a command "docker container exec 8f sh -c 'tail -f ./text.log'" where 8f are the first two characters of the container ID.

![alt text](https://github.com/JariRintaaho/DevOps-with-Docker-HY/blob/main/Part1/figs/Fig_1_5_part2.PNG)

The secret message was "You can find the source code here: https://github.com/docker-hy"
