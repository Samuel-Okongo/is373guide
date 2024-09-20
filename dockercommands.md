1. Building the Docker Image

Start by building the Docker image using your Dockerfile. This step packages your application and dependencies into a container image.

bash
Copy code
docker build -t <image-name> .
-t <image-name>: This option tags your image with a name (replace <image-name> with a meaningful name for your project).
.: Specifies that Docker should look for the Dockerfile in the current directory.
Example:

bash
Copy code
docker build -t my-website .
2. Running the Docker Container

Once the image is built, you can run it as a container. This step launches your application in an isolated environment.

bash
Copy code
docker run -d -p <host-port>:<container-port> <image-name>
-d: Runs the container in detached mode (in the background).
-p <host-port>:<container-port>: Maps a port on your local machine to a port inside the container (replace <host-port> and <container-port> with actual port numbers).
<image-name>: The name of the image you built earlier.
Example:

bash
Copy code
docker run -d -p 8080:80 my-website
This command makes your website available at http://localhost:8080.

3. Listing Running Containers

To see which containers are currently running, use:

bash
Copy code
docker ps
This command will show you the container ID, image name, ports, and other useful information about your running containers.

4. Stopping a Container

To stop a running container, use the docker stop command followed by the container ID or name:

bash
Copy code
docker stop <container-id>
Example:

bash
Copy code
docker stop abc123def456
You can find the container ID by using the docker ps command.

5. Removing a Container

Once a container is stopped, you can remove it with the following command:

bash
Copy code
docker rm <container-id>
Example:

bash
Copy code
docker rm abc123def456
6. Viewing Logs

If you need to troubleshoot or check the logs of a running container, use:

bash
Copy code
docker logs <container-id>
Example:

bash
Copy code
docker logs abc123def456
7. Removing Unused Images

Over time, Docker images can take up space. You can remove unused images with this command:

bash
Copy code
docker image prune
8. Cleaning Up Everything (Containers, Images, Volumes)

If you want to remove all containers, images, volumes, and networks not currently in use, you can use the following command:

bash
Copy code
docker system prune -a
-a: This removes all unused images in addition to containers, volumes, and networks.
9. Accessing a Running Container (Optional)

If you need to open a terminal within a running container (to debug or modify something), you can use docker exec:

bash
Copy code
docker exec -it <container-id> /bin/bash
This command opens an interactive shell inside the container.

10. Docker Compose (Optional)

If your project grows and you need to run multiple services (like a database alongside your web app), consider using Docker Compose. Here’s a basic example of a docker-compose.yml file:

yaml
Copy code
version: '3'

services:
  web:
    image: nginx:alpine
    ports:
      - "8080:80"
    volumes:
      - ./src:/usr/share/nginx/html
Run it with:

bash
Copy code
docker-compose up -d
Summary of Useful Docker Commands

Here’s a quick recap of the commands mentioned in this guide:

Build Image: docker build -t <image-name> .
Run Container: docker run -d -p <host-port>:<container-port> <image-name>
Stop Container: docker stop <container-id>
Remove Container: docker rm <container-id>
View Logs: docker logs <container-id>
Prune Images: docker image prune
Full Cleanup: docker system prune -a
