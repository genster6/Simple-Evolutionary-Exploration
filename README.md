# Simple Evolutionary Exploration
---
## Overview  

As technology advances, image data is becoming a common element of research experiments. Studies in everything from self-driving vehicles to plant biology utilize images in some capacity. However, every image analysis problem is different and processing this kind of data and retrieving specific information can be extremely time consuming. Even if a researcher already possesses knowledge in image understanding, it can be time consuming to write and validate a customized solution. Thus, if this process can be automated, a significant amount of researcher time can be recovered. The goal of this project will be to generate and develop an easy-to-use tool that can achieve this automation for image segmentation problems.  

In order to achieve this goal, this project will utilize the power of genetic algorithms. Genetic algorithms apply concepts of evolutionary biology to computational problems. This allows them to have several strengths over other methods including, but not limited to, being simple to implement, having flexible implementation that can adapt easily to different workflows, and having final solutions that are easily interpreted by humans. One way to think of genetic algorithms is as machine learning for machine learning. When presented with an example image, the genetic algorithm will not only find the best image segmentation algorithm to use, but will also find the optimal parameters for that specific algorithm.  

---
## Project Description  

For this project, many of the components necessary already exist. The general genetic algorithm code has already been constructed and has been rewritten into an easy-to-use format. The code exists in a state that is easy to use with Jupyter notebooks as well. However, several key pieces are still missing. Two major parts of genetic algorithms are the fitness function and the genetic representation vector. The fitness function, or measure of error, is mostly finished, although it does still need to be slightly refined. The genetic representation vector, or the search space, currently works but is constructed in a basic way and is subsequently very large. A smaller search space will aid the algorithm in achieving better performance. As part of this project I will aim to refine the fitness function and shrink the overall size of the search space.  

I also hope to clean up the overall code, and package it in a way that makes it easy for others to use. This includes an intuitive user experience and an immediately usable output. Since the genetic algorithm outputs a specific segmentation algorithm with optimal parameters, it is reasonable to believe we could make it output Python code to perform the segmentation process. All the user would have to do is copy the code into a Python script or Jupyter cell, and everything would run automatically from there. 

---

### Dependencies
* python 3.7.6 
  * [conda 4.8.3](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)
  * [jupyter 4.6.1](https://jupyter.readthedocs.io/en/latest/install.html)
* [numpy 1.18.1](https://anaconda.org/anaconda/numpy)
* [matplotlib 3.1.3](https://matplotlib.org/users/installing.html)
* [scikit-image 0.16.2](https://scikit-image.org/docs/dev/install.html)
  * skimage.segmentation
* [deap 1.3](https://anaconda.org/conda-forge/deap)
* [scoop 0.7](https://scoop.readthedocs.io/en/0.7/install.html)
* [cv2 4.2](https://docs.opencv.org/master/da/df6/tutorial_py_table_of_contents_setup.html)

Dependencies can be installed manually, or by creating a conda environment using the command below:  

**Windows:**  

	conda env create --prefix ./envs --file environment_Windows.yml

**MacOS and Linux:**  

	conda env create --prefix ./envs --file environment.yml


