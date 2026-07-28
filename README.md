# CCPBioSim Protein Analysis Workshop

[![ci](https://github.com/ccpbiosim/protein-analysis-workshop/actions/workflows/build.yaml/badge.svg?branch=main)](https://github.com/ccpbiosim/protein-analysis-workshop/actions/workflows/build.yaml)
[![latest](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fccpbiosim.github.io%2Fassets.json&query=%24.containers.protein-analysis-workshop.latest&labelColor=grey&logo=github&logoColor=white&label=latest&color=purple)](https://github.com/ccpbiosim/protein-analysis-workshop/pkgs/container/protein-analysis-workshop)
[![issues](https://img.shields.io/github/issues/ccpbiosim/protein-analysis-workshop?logo=github&labelColor=grey)](https://github.com/CCPBioSim/protein-analysis-workshop/issues)
[![pr](https://img.shields.io/github/issues-pr/ccpbiosim/protein-analysis-workshop?logo=github&labelColor=grey)](https://github.com/CCPBioSim/protein-analysis-workshop/pulls)

This workshop source repository contains the build recipe for a docker container derived from the CCPBioSim JupyterHub image. This container adds the necessary software packages and notebook content to form a deployable course container.

This workshop introduces the application of MDTraj to the analysis of protein simulation data

It is in two parts:

1. INTRODUCTION
An introduction to the use of MDTraj for the analysis of simulations. The data comes from the associated 'protein simulation with amber and openmm' workshop.

2. EQUILIBRATION
An introduction to a key issue in MD simulation: testing for equilibration, sampling, and convergence. The data here comes from a long simulation of a different protein, chignolin.

## How to Use

This training course is deployed on the [CCPBioSim](www.ccpbiosim.ac.uk) website via our cloud infrastructure, however you can deploy on your own machine with docker.

Pull the container from our repository::

    docker pull ghcr.io/ccpbiosim/protein-analysis-workshop:latest

In our containers we are using the JupyterHub default port 8888, so you should
forward this port when deploying locally::

    docker run -p 8888:8888 ghcr.io/ccpbiosim/protein-analysis-workshop:latest

## Authors

Workshop Content Authors:

- Charlie Laughton

## Contact

Please direct all questions and feedback to [Charlie Laughton](mailto:charles.laughton@nottingham.ac.uk)
