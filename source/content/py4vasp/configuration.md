Configuration
============

**Conda environment and configuration**

1. Create and activate virtual environment

   ```bash
   conda create -n env_name python
   conda activate env_name
   ```

2. Install `ipykernel` in the environment where the kernel needs to be added, `env_name` is the name of the virtual environment to use the kernel, and `kernel_name` is the name that will be displayed in JupyterLab

   ```bash
   python -m pip install ipykernel
   python -m ipykernel install --user --name env_name --display "kernel name"
   ```

3. Check or uninstall the kernel

   ```bash
   jupyter kernelspec list
   jupyter kernelspec uninstall kernel_name
   ```

   

**Installation of py4vasp**

1. Install using `pip` in the environment have been configured

   ```bash
   python -m pip install py4vasp
   ```

2. There was a problem reported when `import py4vasp` [[link](https://www.vasp.at/forum/viewtopic.php?t=18626)], which caused by the incompatible version of `ipywidgets`  or `nglview`.

   ```bash
   python -m pip install ipywidgets==7.6.1
   ```




> **_NOTE:_** `ipywidgets`: A python library of HTML interactive widgets for [IPython/Jupyter](http://jupyter.org/). [[link](https://ipywidgets.readthedocs.io/en/stable/)]
>
> ​			`nglview`: An [IPython/Jupyter](http://jupyter.org/) widget to interactively view molecular structures and trajectories. [[link](https://github.com/nglviewer/nglview)]
>
> ​			 

