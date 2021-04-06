# 🐳 Docker-For-Django Starter Files 🐳

### Dockerize an existing Django project
or
### Create a Docker container with a new Django project

&nbsp;
## Why django into a docker container ?

#### For development or production , there are many reasons you might want to use django into a Docker container, here are few :


- SMOOTH INTEGRATION 😎 : Using docker, you can create your own tailored environment. Very easily, you can then share it, as a common working base, accross your network of friends and collaborators. The behavior of your contained files will remain the same, whichever OS or computer you are operating from, bringing CROSSCOMPATIBILITY to the next level 🌎 

- LIGHT AND FAST : To work with django in Linux environment, you might have had to setup a dualboot or a VM on your system. This can be time and ressource consumming. Creating an environment through docker, will take at most few minutes and result in a lightweight fast image, sparing your RAM capacity 🐏  

&nbsp;
## Let's make it work ! Only 2 command lines required 🙏

### Install Dokcer Engine (if not already)

Official documentation is well made [https://docs.docker.com/engine/install/](https://docs.docker.com/engine/install/)

- If operating on Windows, make sure to have WLS2 installed ( a prompt will let you know in due time, otherwise [here](https://docs.microsoft.com/en-us/windows/wsl/install-win10#step-4---download-the-linux-kernel-update-package) )
- If operating on linux make sur to install the docker-compose agent, it comes as default on windows and mac Docker Engine. See official doc if needed [here](https://docs.docker.com/compose/install/) 

&nbsp;
&nbsp;

### If you want to create a new django project 🐍
&nbsp;

Make a new directory, and copy into it the 3 files from Docker-For-Django-Starter-Files. You structure should be :

* MyDirectory
 
  * Dockerfile
  * docker-compose.yml
  * requirements.txt ( optional : Specify a django version and other dependencies you might need )

Then open a terminal in this directory and run :
```{bash}
docker-compose run web django-admin startproject <yourprojectname> .
```
  _Don't forget the point . at the end of the command_ 😉
  
&nbsp;
  
  
Congratulations !!! Your new django project has been created, you can navigate the files through your favorite IDE ! 

Now to get your test server up and running, on your port 8000 ( localhost:8000 ), run the following command :
```{bash}
docker-compose up
```

Here you go ! 🚀🚀🚀


## Coming next how to easily set up a django existing project with these docker files 







