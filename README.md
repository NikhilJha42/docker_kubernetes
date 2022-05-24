# docker_kubernetes
Repository for learning Docker and Kubernetes.

## Microservices Architecture
- Made up, somewhat unsuprisingly, from microservices.
- These are distinct specialised units of services or servers that communicate via APIs, and together form the entire application.
- This allows different parts of the network to be tested/debugged/changed without affecting the application until they are ready for deployment.
- E.g., an online shop such as Amazon has a login page, different item categories, a basket, payment page, and databases to store information, which are all microservices.
- A local online shop would have a monolithic architecture - that is, all parts of the application would exist on one server.

## Containerisation (with Docker)
- Containerisation is the packaging of code and dependencies into an isolated, light-weight container, which can then be run on (ideally) ANY local machine.
- A container doesn't contain anything more than an app and its running environment - whereas a virtual machine has an OS, CPU, etc. and is therefore much larger. 
- In particular, containerisation is more useful for microservice architectures, whereas VMs are more useful for monolithic architectures.
- Docker is a containerisation tool that works wiht Windows, Mac and Linux machines.
- Docker container lifecycle: build, run, stop, start, (and so on) until destroy.
- Docker uses a REST API to pull images from docker with which to build containers - these are immutable instructions on how to build a container with specific dependencies and code.
- Docker daemon listens for Docker API requests and manages Docker objects.
- Advantages of Docker: open-source (with a variety of images available), easy interface, automated container creation.
