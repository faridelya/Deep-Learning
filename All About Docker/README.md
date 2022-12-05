This directory contain all about docker
- Rule of thumbs.
 > Always use the same CUDA and cuDNN version in Docker image as present in the underlying host machine.
 > Don’t blindly install latest tensorflow/pytorch library from PyPi. It is absolutely incorrect that any version of this both package will work with any version of CUDA, cuDNN. In fact, the combination of the latest version of both, tensorflow/pytorch with CUDA/cuDNN may not be compatible. Always test the combination in a development environment first.
 > Docker hub of Nvidia has a lot of images, so understanding their tags and selecting the correct image is the most important building block. The description from official Nvidia docker hub is,
 
1. [A complete guide to building a Docker Image serving a Machine learning system in Production](https://towardsdatascience.com/a-complete-guide-to-building-a-docker-image-serving-a-machine-learning-system-in-production-d8b5b0533bde)

1.  [Containers with CUDA support](https://lpryszcz.medium.com/containers-with-cuda-support-5467f393649f)

> To use docker container with GPu you have to install NVIDIA CONTAINER TOOLKIT.
 
2. [NVIDIA CONTAINER TOOLKIT](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html)
3. [Enabling GPU access with Compose](https://docs.docker.com/compose/gpu-support/)
