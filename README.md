# Welcome to Docker

This is a repo for new users getting started with Docker.

You can try it out using the following command.
```
docker run -d -p 8088:80 --name welcome-to-docker docker/welcome-to-docker
```
And open `http://localhost:8088` in your browser.

# Building

Maintainers should see [MAINTAINERS.md](MAINTAINERS.md).

Build and run:
```
docker build -t welcome-to-docker . 
docker run -d -p 8088:3000 --name welcome-to-docker welcome-to-docker
```
Open `http://localhost:8088` in your browser.

#How do I run a container
```
Steps: 
1. In this guide, you create an image using a Dockerfile and a sample application.
2. Open the sample application in your IDE. Note that it already has a Dockerfile. For your own projects you need to create this yourself.
3. You can build an image using the following docker build command via a CLI in your project folder.
    > docker build -t welcome-to-docker .
    Breaking down this command
    The -t flag tags your image with a name. (welcome-to-docker in this case). And the . lets Docker know where it can find the Dockerfile.
4. Once the build is complete, an image will appear in the Images tab. Select the image name to see its details. Select Run to run it as a container.
5. You now have a running container. If you don't have a name for your container, Docker provides one. View your container live by selecting the link below the container's name in your Docker Desktop.
```
