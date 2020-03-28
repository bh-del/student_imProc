---
title: xxx
...

# Preparing the computer for the laboratory

1. Install Anaconda distribution - see section 3.
2. Install text editor with Python syntax support - for Windows, e.g. [notepad++](https://notepad-plus-plus.org/).
3. Install editor with *markdown* support:

   - plugin to the *notepad++* editor 
   - [Mark Text](https://github.com/marktext/marktext)


# Anaconda 

What is Anaconda?  
   > It is generally speaking platform for scientific calculations - see [here](https://www.anaconda.com/what-is-anaconda/)
    
What is conda?  
   >It is a system for package and environment management open source licenseded - see [here](https://conda.io/docs/)
  
Anaconda Didtribution:  see [here](https://www.anaconda.com/distribution/)


## Installing

1. Download the chosen installation [package](https://www.anaconda.com/download/#download):

    - select your operation system ie. Windows:
    - choose the default version of python 3

2. Run the installation and follow the appearing tips:

    - for Windows: [install](http://docs.anaconda.com/anaconda/install/windows/)
    - for Linux: [install](https://docs.anaconda.com/anaconda/install/linux/)

3. After installing Anaconda:

    - run Anaconda terminal on Windows:
    - run terminal on Linux
    - check conda version:  `conda –version `
    - update conda manager:  `conda update conda  `
    - update of Anaconde:  `conda update anaconda`



# Conda environments and packages management

## Management of environments

For each project we advice to create separate environment with installed needed packages. Basic commands [help]( https://conda.io/docs/user-guide/tasks/manage-environments.html):

   > **conda create  -n name_of_environment** - create an environment called name_of_environment  
       **conda create -n name_of_environment python=3.6.6** - create an environment called name_of_environment, with the indicated Python version  
       **conda remove -n name_of_environment** –all environment remove  
       **activate name_of_environment** - activating the environment on Windows  
      ** conda activate name_of_environment** - activating the environment on Linux  
      ** deactivate deactivating** - the environment on Windows  
      ** conda deactivate deactivating** - the environment on Linux  
      ** conda info –envs / conda info -e** - displaying a list of available environments  
       

## Packages management

Basic commands [help]( https://conda.io/docs/user-guide/tasks/manage-pkgs.html):  

   > **conda list** - check the list installed packages in current environment sprawdzenie  
   > **conda list | findstr package_name** - search for packages installed in the current environment using the stream | and console command **findstr** - on Windows  
   > **conda list | grep package_name** - search for packages installed in the current environment using the stream | and console command **grep** - on Linux  
   > **conda install package_name** - installs package in current environment  
   > **conda remove package_name** - remove package from current environment  



## Tools

Ipython:
   > It is interacitive console of Python language - see [here](https://ipython.readthedocs.io/en/stable/)


Jupyter notebook:
   > kkk
