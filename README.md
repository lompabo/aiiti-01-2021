---
title: AI in the Industry Tutorials (Density Estimation for Anomaly Detection)
author: michele.lombardi2@unibo.it
---

# AI in the Industry Tutorials: Density Estimation for Anomaly Detection #

This is one of a series of tutorials that are part of the "AI in the Industry" course at [University of Bologna](https://www.unibo.it/it). Each tutorial tackles a simplified industrial problem and aims at showing how similar problem can be tackled using AI techniques, from Machine Learning to Combinatorial Optimization (and later on their combination).

This tutorial in particular tackles a simple anomaly detection task via density estimation techniques. The focus is on building an end-to-end solution, where calibrating the detection threshold can be as important as building the density estimation model itself.

# Accessing the Tutorial #

The tutorial is split over multiple (numbered) Jupyter notebooks. _The preferred way to access the tutorial is via Binder_, which enables running the code on a remote server:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lompabo/aiiti-01-2021/HEAD)

Alternatively, it is possible to _inspect the notebooks in a static form_ (by just clicking on any `*.ipynb` file in this directory), or to _run the code locally_. Doing this will require to:

* Install Docker, by following the [online instructions](https://docs.docker.com/get-docker/).
* Install Docker Compose, by following the [online
instructions](https://docs.docker.com/compose/install/)
* Clone the repository with the tutorial, in this case via the command:
```sh
git clone https://github.com/lompabo/tutorial-template-python.git
```
* Start the container via Docker Compose, from the main directory of the
tutorial:
```sh
docker-compose up
```

On linux systems, you may need to start the docker service first.

The first execution of this process will be fairly long, since Docker will
need to download a base image for the container (think of a virtual machine
disk) and then some boilerplate configuration steps will need to be performed
(e.g. installing jupyter in the container). Subsequent runs will be much
faster.

The process will end with a message such as this one:
```sh
To access the notebook, open this file in a browser:
    file:///home/lompa/.local/share/jupyter/runtime/nbserver-1-open.html
Or copy and paste this URL:
    http://127.0.0.1:39281/?token=0cd92163797c3b3abe67c2b0aea57939867477d6068708a2
```
Copying one of the two addresses in a file browser file provide access to the Jupyter server running in the spawned container.

Once you are done, pressing CTRL+C on the terminal will close the Docker container.

For more information about how Docker works (such as the difference between
images and containers, or how to get rid of all of them once you are done with
the tutorial), you can check the [Docker
documentation](https://docs.docker.com/).
