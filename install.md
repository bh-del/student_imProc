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

   - `conda create  -n name_of_environment` - create an environment called name_of_environment
   - `conda create -n name_of_environment python=3.6.6` - create an environment called name_of_environment, with the indicated Python version
  
   - `conda remove -n name_of_environment` –all environment remove
   - `activate name_of_environment*` - activating the environment on Windows
   - `conda activate name_of_environment` - activating the environment on Linux
   - `deactivate deactivating`- the environment on Windows
   - `conda deactivate deactivating` - the environment on Linux
   - `conda info –envs / conda info -e` - displaying a list of available environments
       

## Packages management

Basic commands [help]( https://conda.io/docs/user-guide/tasks/manage-pkgs.html):

   - `conda list` - check the list installed packages in current environment sprawdzenie  
   - `conda list | findstr package_name` - search for packages installed in the current environment using the stream | and console command **findstr** - on Windows  
   - `conda list | grep package_name` - search for packages installed in the current environment using the stream | and console command **grep** - on Linux  
   - `conda install package_name` - installs package in current environment  
   - `conda remove package_name` - remove package from current environment  



# Tools

Ipython:
  >In simple terms, it is a modern, interactive Python interpreter console. In fact, Ipython is something much bigger - [here](https://ipython.org/ipython-doc/stable/overview.html) you can read about it.  

Jupyter Notebook:
   >formerly known as *Ipython Notebok*, it is an interactive computational environment, in which you can combine code execution, rich text, mathematics, plots and rich media. 


## First jupyter notebook

1. First steps: [DataCamp tutorials](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook)
2. Jupiter uses markdown: [Some tutorial](https://commonmark.org/help/)


## Install conda extension

In order to be able to operate virtual environments and collaborate with the *conda* manager from the *Jupyter Notebook* level, an additional package must be installed:

   - run terminal
   - in (base) environment run: *conda install nb_conda*


# Preparation of the environment

## Conda environment

1. Run terminal
2. Create new environment: `conda create -n lab2`
3. Activate environment: `conda activate lab2`
3. Install pakages:

   - numpy: for operations on an array of numbers
   - scipy: image processing functions
   - pillow (PIL): opening image files, image processing functions
     `conda install -c anaconda numpy scipy pillow` 
   - matplotlib: displaying images on the screen
     `conda install -c conda-forge matplotlib`
   - ipykernel: jupyter's packages
     `conda install -c anaconda ipykernel`

## Data

1. Go to page: [ImageProcessingPlace](http://imageprocessingplace.com/root_files_V3/image_databases.htm).
2. Download zip file - fifth (5) row of the table.
3. Create a directory on the disk and extract the images to it.

## Runnig jupyter

1. Start a terminal or deactivate an environment other than 'base' if it is running
2. In the 'base' environment, run: `jupyter notebook`
3. In the opened browser window, go to the directory in which you will work (with images downloaded from the Internet).
4. Click `New` in the upper right corner of the window and select the `lab2` environment. A new notebook window will open.

## Changing the notebook name

1. A notebook file has been created in the working directory: `Untitled.ipynb`
2. Close notepad: menu `File / Close and Halt`
3. In the file browser Jupiter window will know the notebook file and click the `rename` icon in the top menu
4. Rename the notebook file.
5. Launch the notebook by clicking it.
