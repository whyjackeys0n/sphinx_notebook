Metadynamics
============

***Videos***

1. Videos from VASP YouTube channel, *Advanced methods of molecular dynamics* \[[link](https://www.youtube.com/watch?v=HVeamQOmM-s)]

***Parameters***

1. VASP wiki about metadynamics category \[[link](https://www.vasp.at/wiki/index.php/Category:Metadynamics)]
2. [HILLS_H](https://www.vasp.at/wiki/index.php/HILLS_H) (Default = 10<sup>-3</sup> [Real]), sets the height of the Gaussian hills *h* (in eV)
3. [HILLS_W](https://www.vasp.at/wiki/index.php/HILLS_W) (Default = 10<sup>-3</sup> [Real]), sets the width of the Gaussian hills *h* (in units of the corresponding collective variable)
4. [HILLS_BIN](https://www.vasp.at/wiki/index.php/HILLS_BIN) (Default = [NSW](https://www.vasp.at/wiki/index.php/NSW)  [Integer], the number of steps in all ab-initio Molecular Dynamics runs [Integer]), sets the number of steps after which the bias potential is updated in a metadynamics run
5. [SMASS ](https://www.vasp.at/wiki/index.php/SMASS) (Default = -3 [real] or -1, -2, -3), sets the velocities during an ab-initio molecular-dynamics run

* Notes: For a metadynamics run with Nose-Hoover thermostat, one has to set [MDALGO](https://www.vasp.at/wiki/index.php/MDALGO) = 2, and choose an appropriate setting for SMASS. Scripts for calculating SMASS from Qijing Zheng's personal website [[description link](https://qijingzheng.github.io/posts/NVT-MD/)] [[scrips link](https://github.com/QijingZheng/pyband/blob/master/nose_mass.py)]

***Examples using VASP***

1. Nuclephile Substitution CH3Cl - mMD1 \[[link](https://www.vasp.at/wiki/index.php/Nuclephile_Substitution_CH3Cl_-_mMD1)], using one collective variable
2. Nuclephile Substitution CH3Cl - mMD2 \[[link](https://www.vasp.at/wiki/index.php/Nuclephile_Substitution_CH3Cl_-_mMD2)], using extra "repulsive potential walls"
3. Nuclephile Substitution CH3Cl - mMD3 [[link](https://www.vasp.at/wiki/index.php/Nuclephile_Substitution_CH3Cl_-_mMD3)], using two collective variables simultaneously

