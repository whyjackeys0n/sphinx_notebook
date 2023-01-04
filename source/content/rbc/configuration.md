Configuration
============

**ESPResSo Documentation**

1. ESPResSo home website \[[link](https://espressomd.org/wordpress/)]
2. ESPResSo github website \[[link](https://github.com/espressomd/espresso)]
3. ESPResSo documentation (v4.2.0) website \[[link](https://espressomd.github.io/doc4.2.0/index.html)]

**Installation**

1. Execute `sudo apt update` and `sudo apt upgrade` to prepare the installation of dependencies
2. Generate `myconfig.hpp` file from the last build `myconfig-sample.hpp` for the installation.
3. Rename the `myconfig-sample.hpp` file to `myconfig.hpp`, and uncomment `EXTERNAL_FORCES`，`MASS`，`EXCLUSIONS`，`LB_BOUNDARIES`，`SOFT_SPHERE`，`MEMBRANE_COLLISION` and `EXPERIMENTAL_FEATURES`. `EXPERIMENTAL_FEATURES` is the necessary module for `MEMBRANE_COLLISION`.
4. Install ESPResSo using tar.gz format package with command `cmake`, `make` and `sudo make install`.
5. Samples can be directly run under the `sample` directory `~/software/espresso/samples/object_in_fluid` with command `pypresso`.