# JupyterCon JupyterLab Training

This repository contain material and instructions to follow the JupyterLab training during JupyterCon 2018.

During the tutorial, feel free to get on the [Gitter `jupyterlab` channel](https://gitter.im/jupyterlab/jupyterlab) for help and updates.

## Goals
By the end of this training you should be comfortable building multiple kinds of JupyterLab extensions. We will start with building a mimerender extensions, then a full fledged extension, and finally end with an extension that add some new core interface. We will close with Q&A, time permitting.


*Schedule*:

* Installing JupyterLab
* Tour of JupyterLab
* 10:30 Break
* [MP4 Mimerender Tutorial](https://github.com/jupyterlab/jupyterlab-mp4)
* 12:30 Lunch
* [XKCD Tutorial](https://jupyterlab.readthedocs.io/en/stable/developer/xkcd_extension_tutorial.html)
* Toolbar Button Tutorial
* 3:30 Break
* Q & A


## Environment Setup

### Install Miniconda
For this tutorial, we are standardizing on a miniconda-based python distribution.
We may not be able to help with installation issues if
you are using a different python distribution.
First we want to install Miniconda which we will use to manage our Python environment.

This is a quick way to install miniconda locally on Mac or Linux, but refer to the
[Conda installation docs](https://conda.io/docs/user-guide/install/) for reference:

```bash
wget https://repo.continuum.io/miniconda/Miniconda3-3.7.0-Linux-x86_64.sh -O ~/miniconda.sh
bash Miniconda3*.sh -b -p ~/miniconda
source ~/miniconda/bin/activate
```

### Create environment
After you have the `conda` command installed, create an environment for these tutorials called `jupyterlab-ext`: 

```bash
conda create -n jupyterlab-ext nodejs jupyterlab cookiecutter matplotlib scipy ipywidgets python=3.6 -c conda-forge
conda activate jupyterlab-ext
jupyter labextension install @jupyter-widgets/jupyterlab-manager
```

Test if it works by starting JupyterLab `jupyter lab`.
