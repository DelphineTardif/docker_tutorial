# Introduction

A small demo project to reproduce figures in a notebook

# How to run code
## From source code
1. Download code
2. `docker build -t my-totebook .` builds the image locally
3. `docker run -it -p 8888:8888 my-totebook`Run a container from locally built image

## From the web 
1. `docker run -it -p 8888:8888 wesleyban/docker_presentation`Run a container from locally built image pushed to the Web.

# Using your own data 
it's possible to use your own data. You must mount a volume into the contained as so: 
`docker run -it -p 8888:8888 -v $PWD/resultats:/home/jovyan/work/resultats my-totebook`
It is paramount to use absoluto Path. 
Beware: when closing session, the modifications on the image will be delted (to be checked)



