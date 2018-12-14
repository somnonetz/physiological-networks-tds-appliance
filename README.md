# physiological-networks-tds-appliance

Dockerfile for the physiological network tds appliance description 

# Application

Physiological network TDS is an implementation of the Time Delay Stability algorithm, introduced by Bashan et al. ([doi:10.1038/ncomms1705](https://doi.org/10.1038/ncomms1705)). It can be used in sleep research to determine the topology of the physiological networks by analysis of a polysomnographic recording. The physiological network tds software is developed at CBMI (HTW Berlin - University of Applied Sciences), and is available as matlab code on github [physiological-networks-tds]https://github.com/somnonetz/physiological-networks-tds).

# Appliance

This repo contains the Dockerfile to build the appliance. 
The application is packaged as [Curious Containers](https://www.curious-containers.cc) compatible Docker image.
Furthermore, the repo contains the recipe to build the appliance with a meaningful name and to push it into the 
 official [DockerHub](https://hub.docker.com/r/curiouscontainers/cc-tds-app/) registry. Credentials are required.

# Getting Started

## Prerequisites

To build the image, you need a Docker installation on your system.
As you require the full 1.4 GB Matlab mcr within the Docker image, a fast internet connection is highly recommended. 
If you want to run the appliance, you need cc-faice and an experiment description containing this Docker image. 
Examples can be found in the repective repository:
[physiological-networks-tds-experiments](https://github.com/somnonetz/physiological-networks-tds-experiments)


## Build the appliance

1. Clone the repo:

   git clone https://github.com/somnonetz/physiological-networks-tds-appliance
   
2. Move into the directory physiological-networks-tds-appliance
   
   cd physiological-networks-tds-appliance
   
3. Build the Docker image

    docker build .


