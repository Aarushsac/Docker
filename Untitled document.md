**Docker**  
What is Docker?  
Docker is a platform that provides tools and services for creating,updating and deleting containers which help us solve a problem which many developers face when in large teams to replicate local environment of systems.Docker helps us to solve this issue and thus solves an essential part of development process.

What does a container contain?  
A container contains the code of the application or website along with all the dependencies required to run that application.

Problem solved by Docker  
Supposingly,now we are creating a website or an application and we have our local system and code written on it and we have installed some dependencies related for running the code in our system.Now, there is a certain part of code which runs with node v16 and redis v6 in our system to run our application.It is not compliant with any previous or newer versions only with current versions.Plus our code also contains some Commands Line Interface commands which are specific to our Linux system and won’t work with Mac OS or Windows.Now we are working in a large team a new teammate joins we want he should be able to work on this application and for that he has to setup the same environment as the one in my system.He now manually set’s up all the dependencies and in that process he downloads and installs v20 of node and v7 of redis.Now these versions don’t support the feature of our code.This makes a issue or error arise when the new teammate tries to work on the application.Even he has a different OS so he is not able to work with the same CLI commands and needs different to work on it.This problem was faced by many developers and had to be addressed and a solution to this problem was the platform Docker.

Docker is a platform that helps build containers.Now all the code of the application or website and it’s dependencies are packed into a single unit called as Container.Now these shared with following developers.

**Features of Container:-**  
**1.Portable**  
The containers are portable in the sense that they can be shared and used on devices with different Operating Systems.  
**2.Lightweight**  
These containers are easy to build,update and destroy.

A container is an isolated computing environment built in a local system which is separate from the system and can carry the whole development process inside it.

**Docker Image**  
A docker image is a screenshot or snapshot of what the code and dependencies look like or what the local environment of the system looks like.

We don’t share the containers to fellow team members we share docker images with other team mates they download the images and make containers through these images.

Images and containers are like classes and objects analogy.

The images do not contain any resources the containers contain the resources the classes contain the blueprint of the object and the object are instances of the classes.

We make images of our project or applications and their dependencies and these images are shared.

These images contain the code and the dependencies.  
Dockerhub is like github where images are uploaded and can be downloaded or installed by other developers.

Pull command is used to extract the image from dockerhub to our local system docker desktop.

Now for converting an image to a container and running the container we use the following command:-  
**Docker run image\_name**

**Docker daemon** is the main component of docker desktop which is responsible for all the functionalities of the docker desktop.

We use **docker run \-it image\_name** for running containers in interactive mode these containers contain applications which are using some command line interface commands for further running or processing.

**Exit command is used for exiting the application.**  
**Docker stop container\_id to stop the container process.**

Docker only virtualizes the application layer and shows the local system of the application or replica of the system in the application layer.  
