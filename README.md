# JupyterCon JupyterLab Extension Training

## Goals

* Get you comfortable building JupyterLab extensions
  * Renderer
  * Free form
  * Extending interface
* Answer any questions you have about JupyterLab


## Schedule
* Installing JupyterLab
* Tour of JupyterLab
* 10:30 Break
* [MP4 Mimerender Tutorial](https://github.com/jupyterlab/jupyterlab-mp4)
* 12:30 Lunch
* [XKCD Tutorial](https://jupyterlab.readthedocs.io/en/stable/developer/xkcd_extension_tutorial.html)
* Toolbar Button Tutorial
* 3:30 Break
* Q & A


## Setup your environment

### Install Miniconda
First we want to install Miniconda which we will use to manage our Python environment:

[Mac/Linux](https://conda.io/docs/user-guide/install/macos.html#install-macos-silent):

```bash
wget https://repo.continuum.io/miniconda/Miniconda3-3.7.0-Linux-x86_64.sh -O ~/miniconda.sh
bash Miniconda3*.sh -b -p ~/miniconda
source ~/miniconda/bin/activate
```

[Windows](https://conda.io/docs/user-guide/install/windows.html#install-win-silent)

### Create environment
After you have the `conda` command installed, create an environment for these tutorials called `jupyterlab-ext`: 

```bash
conda create -n jupyterlab-ext nodejs jupyterlab cookiecutter matplotlib scipy ipywidgets -c conda-forge
conda activate jupyterlab-ext
jupyter labextension install @jupyter-widgets/jupyterlab-manager
```

Test if it works by running `jplm --version`.
