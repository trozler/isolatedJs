### Aprroach

In order to run an arbitrary JS file in a secure context we need to utilse some level of virtualisation. We will use container for virtualisation as they are relativly lightweight and easy to use. Unlike Virtual machines which virtualise the hardwear, containers virtualise the OS.

Containers run images, which are a snapshots of your code and its dependencies. these images contain everything needed to run your project in any envrionment (assuming environment runs docker).

You build your images using docker files. These files act a build configurationfiles for the docker engine which buids your image.

Once you have an image you can run it in a container.

1. We will create a docker file that creates an image which can run an arbitrary javascript file.
2. We we run the image we will copy the javascript file into the docker file system.
3. The container will execute the file and return the result to our program.

### Dependency

Assumes you have docker installed.
