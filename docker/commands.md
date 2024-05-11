1. Below command is used to run the container locally and if the container is already not
   present locally it pulls from the docker hub

        docker run nginx
2. List all running containers

        docker ps 
3. List all containers

        docker ps -a
4. Stop the container

        docker stop <container-name>
5. To see the list of the images

        docker images
6. To remove images from the container. Before removing the image make sure no container is dependent on it

         docker rmi <image-name>
7. Only pull images from the docker hub.

         docker pull <image-name>

> **Note:** if the webservices inside the container is stopped or chash then container also exists.

8. To list all the files inside the running container.

         docker exec <image-name> cat /etc/hosts
9. **Attach and detach** To run the container in the detached mode. As by default the console is occupied and you can 
 not exit out. So its better to run it in the detach mode.

         docker run -d <image-name>
10. To attach back the container

         docker attach <container-id>
11. 