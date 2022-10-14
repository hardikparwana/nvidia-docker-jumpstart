## NVIDIA docker images
The Dockerfiles have been tested on Ubuntu 22.04

### CUDA 11.6 Ubuntu 20 image:
```
FROM hardikparwana/cuda116desktop:v1
```
The Cuda 11.6 image is built from nvidia/cuda:11.6.1-cudnn8-devel-ubuntu20.04. This image does not have graphics libraries installed though. Docker compose build for `apt install gedit` (to install all graphics related libraries) didn't work as I was unable to send commands from keyboard when prompted for setting the time zone, region, etc. Therefore, starting with nvidia image, graphics libraries were installed without docker compose by installing gedit. The final image was pushed to docker.io.
