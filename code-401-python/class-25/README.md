# Docker

## Docker is really just Linux containers which are a type of virtualization.

# Docker's functionality : 
###  A way to implement Linux containers!

### An analogy we can use here is that of homes and apartments. Virtual Machines are like homes: stand-alone buildings with their own infrastructure including plumbing and heating, as well as a kitchen, bathrooms, bedrooms, and so on. Docker containers are like apartments: they share common infrastructure like plumbing and heating, but come in various sizes that match the exact needs of an owner. 

## Diff between Containers and Virtual Environments:
### Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer.

### virtual environments can only isolate Python packages. They still rely on a global, system-level installation of Python albeit they can refer to the proper version. So when we use Python 2.7 in a project, we’re pointing to an installation of Python 2.7 on the computer itself, not actually within the virtual environment.

### Also we can’t run a production database or other services within virtual environments so compared to Docker containers they are far more limited.

## Commands : 
 - docker run hello-world : This will download an official image and then run the container.
 - docker info : give me the info for docker.
 - docker image ls : Want to inspect just the current image.
 
## Images and Containers
### Images and containers are the two fundamental concepts to grasp when you start with Docker. An image is a snapshot in time of what a project contains. A container is a running instance of the image.

### When we ran hello-world we used an official Docker image. We did not have to create the image ourself. But typically we will create custom images and we do so using a Dockerfile. We also will use docker-compose.yml files to run the containers.


## Containers
### Now that we have our Python image how do we run it? Well just as a Dockerfile is a list of image instructions there is also a docker-compose.yml file that is a list of container instructions.

### To demonstrate a real-world image and container example we will now “Dockerize” a basic Django web app. You might not fully understand every step but you’ll see how Docker can work to run a web application completely on its own.


- Docker is a way to run Linux containers
- Containers are a lightweight alternative to Virtual Machines
- Dockerfile is a list of instructions for creating an image
- Images are made up of one or more layers
- Containers are a running instance of an image
- docker-compose.yml controls how to run the container
- Containers are stateless and ephemeral in nature. We can link the local filesystem via volumes but things become more - - complex with databases (which we didn’t cover here).


## Build out a Library website and API with Django/Django REST Framework:

### Django REST Framework works alongside the Django web framework to create web APIs. We cannot build a web API with only Django Rest Framework. It always must be added to a project after Django itself has been installed and configured.

##  similarities and differences between traditional Django and Django REST Framework:

### The most important takeaway is that Django creates websites containing webpages, while Django REST Framework creates web APIs which are a collection of URL endpoints containing available HTTP verbs that return JSON.


