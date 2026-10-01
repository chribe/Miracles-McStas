This repository contains the MCStas file for the neutron backscattering spectrometer MIRACLES at the ESS.
The McStas code in the file ESS_MIRACLES.instr can be run via standard mcstas commands such as 

mcrun --format=NeXus ESS_MIRACLES_v11_tubes.instr chopperfile=choppers_hires.cfg SRC_MIN=6.5 SRC_MAX=7 -n 1e9

Chopper settings (frequency and phase) are saved in the file choppers_hires.cfg. If the mcstas code is run saving the data in a nexus file, the chopper settigns are saved within the nexus structure, so that the values can be used in the data reduction.

In case the simulations should be run via the run_simulations.ipynb notebook, the mcstas model has first to be opened via the mcgui and the python folder has to be created via the Pylab button before the notebook can be run.
