# Part 1

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

First the CONTAINER ID was checked using a command "docker container ls" The first two characters were "f0" The secret message was revealed with a command "docker container exec f0 tail -f ./text.log" The secret message was "You can find the source code here: https://github.com/docker-hy"

![alt text](https://github.com/JariRintaaho/DevOps-with-Docker-HY/blob/main/Part1/figs/Fig_1_3_part2.PNG)


## Task 1.4

Commands:
- docker run -it ubuntu
