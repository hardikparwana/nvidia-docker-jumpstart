## NVIDIA docker images
The Dockerfiles have been tested on Ubuntu 22.04

### CUDA 11.6 Ubuntu 20 image:
The Cuda 11.6 image is built from nvidia/cuda:11.6.1-cudnn8-devel-ubuntu20.04. To get the graphics going though, had to install all the graphics libraries and setting the time zone on prompt didn't work with docker compose build. Therefore, starting with nvidia image, graphics libraries were installed without docker compose by installing gedit. The final image was pushed to docker.io. This image was finally used in th Dockerfile
