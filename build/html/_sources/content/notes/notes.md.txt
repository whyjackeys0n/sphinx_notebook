Notes
============

**Whether XDATCAR is wrapped**


Projecting back to the first cell only happens in relaxations and MD simulations using **MDALGO=0**. For any **MDALGO>0**, the atoms propagate freely.

1. VASP forums - [The ionic coordinates in XDATCAR is wrapped or unwrapped](https://www.vasp.at/forum/viewtopic.php?t=17556)
2. VASP forums - [AIMD XDATCAR wrap and unwrap problems](https://www.vasp.at/forum/viewtopic.php?f=4&t=18667)

**Codes for XDATCAR unwrapping**

1. From [Liren Liu's Notebook](https://lirens-notebook.readthedocs.io/en/latest/scripts/python_scripts/python_msd.html)

2. From [Pai Li's Notebook](http://home.ustc.edu.cn/~lipai/scripts/ml_scripts/xdat2xyz_unwraped.html)