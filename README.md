# Docker
Docker is a platform that allows you to package an application along with everything it needs (code, libraries, dependencies, environment) into a container, so it runs the same everywhere.

## Components of Docker

### Docker Engine:
Docker Engine has a core part docker daemon , that handles the creation and management of containers.
### Docker Image:
Docker Image is a read-only template that is used for creating containers, containing the application code and dependencies, while a container is a running instance of that image. image is a blue print we can create many container 
### Containers: 
Standardized, isolated runtime instances created from an image. They are lightweight because they share the host operating system's kernel, unlike virtual machines which run a full guest OS. A container is a running instance created from an image.

### When you run:

Docker Engine: we write Instructions to build an image, Steps to set up the environment
,Commands to run the application code in docker file  which is txt file,used to create image 
1) Takes the image
2) Creates a container from it
3) Starts the application inside that container

# practice with java file
1)create main.java and write some print code
2)create docker file inside the same folder
3)inside docker file write the below 

FROM openjdk:17
WORKDIR /app
COPY . .
RUN javac Main.java
