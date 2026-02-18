# Docker
Docker is a platform that allows you to package an application along with everything it needs (code, libraries, dependencies, environment) into a container, so it runs the same everywhere.

## Components of Docker

### Docker Engine:
Docker Engine has a core part docker daemon , that handles the creation and management of containers.
### Docker Image:
Docker Image is a read-only template that is used for creating containers, containing the application code and dependencies, while a container is a running instance of that image.
### Containers: 
Standardized, isolated runtime instances created from an image. They are lightweight because they share the host operating system's kernel, unlike virtual machines which run a full guest OS. A container is a running instance created from an image.

### When you run:

Docker Engine:
1) Takes the image
2) Creates a container from it
3) Starts the application inside that container
