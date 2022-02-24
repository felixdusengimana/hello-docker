### Simple explanations on docker and how to use it.

`Docker` is open source platform for developing, shipping and running applications.

### Creating docker image

We need to specify `base image`  most often we use  `alpine` 

**Steps**

1. Create a file named `Dockerfile` in base directory
2. Add commands base on what you're interested in example [link](https://github.com/phelixdusengimana/hello-docker/blob/main/Dockerfile)
3. Run this command `docker build -t phelixdusengimana/firstapp`
command explained
<img width="431" alt="image" src="https://user-images.githubusercontent.com/73703812/155483884-1623e990-8b52-4070-b867-e8b4f3894651.png">
The convention for the tag is as follows
<img width="463" alt="image" src="https://user-images.githubusercontent.com/73703812/155484075-75d85b0a-10a6-42d3-8e4f-b4f2bcb2505f.png">
Now run the docker image

Our application running on port 3000 but you cant browse it since this is a container port. How can we 
access our app then?

we use **Container port mapping**
Port mapping is where we map any port on the local machine to container port(s)
The syntax to use while mapping ports is as follows
<img width="500" alt="image" src="https://user-images.githubusercontent.com/73703812/155484459-c44fb0ec-c74b-4630-b5e8-8f9f4dcdf216.png">

Here you go. now to can access our application on localhost.
