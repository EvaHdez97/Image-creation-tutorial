# Tutorial to create a Docker image from a workflow_registry repository and a software catalog

This is a guide on how to create a Docker image using custom workflow registry and software catalog repositories. It will also show how to adapt the source code for image creation, determine the architecture of the PC where the image will be created, modify the image, and export it to "singularity" for use in HPC.

## Repository structure

1. How to determine your processor microarchitecture
2. Download the image creation tutorial from eflows4hpc and customize it
3. How to modify the created image and push it to a Docker Hub repository
4. How to convert a docker image to singularity file
