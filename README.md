# Tutorial to create a Docker image from workflow registry repository and software catalog repository

This is a guide on how to create a Docker image using custom workflow registry and software catalog repositories. It will also show how to adapt the source code for image creation, determine the architecture of the PC where the image will be created, modify the image, and export it to "singularity" for use in HPC.

IMPORTANT: THIS TUTORIAL IS ONLY FOR LINUX/AMD64 AND LINUX/ARM64 PLATFORMS. 
IMPORTANT: If you have PyPI packages and Spack packages listed in your eflows4hpc.yaml, ensure that they are compatible with either linux/amd64 or linux/arm64 architectures.

## Available Architectures

"aarch64", "armv8.1a", "armv8.3a", "armv8.5a", "ppc64", "ppcle", "sparc", "x86", "x86_64",
"x86_64_v3", "x86_64_v2", "x86_64_v4", "arm", "armv8.2a", "armv8.4a", "ppc", "ppc64le", "riscv64", "sparc64", 
"i686", "pentium2", "pentium3", "pentium4", "prescott", "nocona", "nehalem", "sandybridge", "haswell", "skylake",
"cannonlake", "cascadelake", "core2", "westmere", "ivybridge", "broadwell", "mic_knl", "skylake_avx512", "icelake",
"k10", "bulldozer", "piledriver", "zen", "steamroller", "zen2", "zen3", "excavator", "zen4", "power7", "power8",
"power9", "power8le", "power9le", "thunderx2", "a64fx", "cortex_a72", "neoverse_n1", "neoverse_v1", "m1", "m2", "u74mc"

## Repository structure

1. How to prepare the workflow registry repository and software catalog repository
2. How to determine your processor microarchitecture
3. Download the image creation tutorial from eflows4hpc and customize it
4. How to modify the created image and push it to a Docker Hub repository
5. How to convert a docker image to singularity file
6. How to upload a Singularity image to an HPC system and run it (IN PROGRESS)
