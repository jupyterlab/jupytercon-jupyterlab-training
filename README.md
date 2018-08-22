# JupyterCon JupyterLab Training

This repository contain material and instructions to follow the JupyterLab training during JupyterCon 2018.

During the tutorial, feel free to get on the [Gitter `jupyterlab` channel](https://gitter.im/jupyterlab/jupyterlab) for help and updates.

## Goals
By the end of this training you should be comfortable building multiple kinds of JupyterLab extensions. We will start with building a mimerender extensions, then a full fledged extension, and finally end with an extension that add some new core interface. We will close with Q&A, time permitting.


## Schedule

* Installing JupyterLab
* [Tour of JupyterLab](https://github.com/jupyterlab/jupyterlab-demo)
* 10:30 Break
* [MP4 Mimerender Tutorial](https://github.com/jupyterlab/jupyterlab-mp4/blob/master/tutorial.md)
* 12:30 Lunch
* [XKCD Tutorial](https://jupyterlab.readthedocs.io/en/stable/developer/xkcd_extension_tutorial.html)
* [Toolbar Button Tutorial](https://github.com/jupyterlab/runall-extension)
* 3:30 Break
* Q & A


## Environment Setup

For this training, we are standardizing on a miniconda-based python distribution.
We may not be able to help with installation issues if
you are using a different python distribution.

So begin by [installing miniconda](https://conda.io/docs/user-guide/install/) on your system (if you do not have it already).

After you have the `conda` command installed, create an environment for these tutorials called `jupyterlab-ext`: 

```bash
conda create -n jupyterlab-ext nodejs jupyterlab cookiecutter matplotlib scipy ipywidgets python=3.6 -c conda-forge
conda activate jupyterlab-ext
jupyter labextension install @jupyter-widgets/jupyterlab-manager
```

Test that it works by starting JupyterLab `jupyter lab`.


