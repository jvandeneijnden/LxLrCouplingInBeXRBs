# Analysis reproduction repository for the paper "Radio monitoring of transient Be/X-ray binaries and the inflow-outflow coupling of strongly-magnetized accreting neutron stars"

![Lx Lr plane of transient Be/X-ray binaries](Figure6_7/Figure6.png?raw=true "Lx Lr plane of transient Be/X-ray binaries")

## Based on Van den Eijnden et al. (2022), accepted for publication in MNRAS.
## https://arxiv.org/abs/2208.14903

This repository contains a Jupyter notebook and all required underlying data to produce the images in the paper "Radio monitoring of transient Be/X-ray binaries and the inflow-outflow coupling of strongly-magnetized accreting neutron stars". In order to run the Notebook, check the software requirements below, clone the repository, and run through each cell. We refer to the main paper for full details on the data, plots, and MCMC calculations.

Please get in touch via email (jakob.vandeneijnden [at] st-hildas.ox.ac.uk) or github with questions. 

If this repository is useful for your own research, in addition to citing the original paper, please consider including a note to this repository as well.

Prior to re-running the automated X-ray spectral analysis of Swift and NICER observations of 1A 0535+262, please read the README.md file in the folder (NICER_spectra_1A0535p262 and/or Swift_spectra_1A0535p262) carefully; the same goes for the used .tcl script.

Finally, note that plotting Figure 3 can be quite slow on a typical laptop, due to the large filesize of the underlying .fits image. Similarly, fully performing the linmix analysis takes time, but can be sped up by using the pre-calculated output instead.

=======
## Software requirements

This notebook is written in Python2.7; updates to Python3.x should be straightforward but are left to the user (note that this may require an update to linmix as well).

In addition, this notebook makes use of the following packages, where the associated versions were used in the paper calculations. 

- numpy v1.15.4
- matplotlib v2.2.3
- aplpy v1.1.1
- scipy v1.1.0
- astropy v2.0.9
- linmix v0.1.0.dev1
