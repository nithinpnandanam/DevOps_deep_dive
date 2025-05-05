# Intro to containers

* we are not completely utilising the physical servers
* Refer Image 1
* ```hypervisors``` are installed on the physical servers
* they use a concept called ```virtualisation```
* On top of the physical servers we are creating virtual servers
* virtual servers use logical seperation
* we have os for each vm
* on top of the OS we run the application
---
* virtual machines are more secure than contaners
* Reason --> if there are are 5 vm all will have seperate OS.So compete isolation and security
---
* docker is a containerization platform >> used to create containers
* for creating vm we need a virtualization platform [hypervisor]
---
* Refer Image 2
* we can create docker containers in 2 ways
- ```over a physical server```
    * install OS over a physical server
    * then docker can be installed on top of the OS
    * then containers can be created
    * maintenance overhead of the phycical server is an issue
- ```over a vm```
    * More common
    * for one vm we can have several docker containers
---
* docker containers does not have a complete OS
* containers make use of the resource from the base/host OS i.e,[vm or physical server that they are running on]
* the containers will have a minimal OS or base image
* container = **Application + Application dependency + system dependency**
---
* to take image of a vm we take a snpashot : 1GB/2GB
* to take image of a container we take a snpashot : 100MB/500MB
* containers are light weight as they do not have a complete OS
---
* Referm Image 3
* write a docker file
* execute the file and create a docker image
* execute the image and create a container
* commands are given to the ```docker engine``` which does all this
--- 
* docker is so much dependent on docker engine
* so if the engine fails all the containers will be down
* ```Buildah``` solves these kind of issues
---
### Refrence
* [Youtube](https://www.youtube.com/watch?v=7JZP345yVjw&list=PLdpzxOOAlwvIKMhk8WhzN1pYoJ1YU8Csa&index=31)