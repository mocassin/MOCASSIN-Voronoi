## MOCASSIN-Voronoi
[![GitHub license](https://img.shields.io/badge/license-GPL-blue.svg)](https://github.com/mocassin/MOCASSIN-Voronoi/blob/master/LICENSE)

**MOnte CArlo SimulationS of Ionized Nebulae**, Voronoi Version

*3D Monte Carlo Photoionization and Dust Radiative Transfer Code on Voronoi Meshes*

Copyright (C) 2005 Barbara Ercolano

### Installation

How to compile:

    make mocassinVoronoi
    make mocassinWarm
    make mocassinOutput
    make mocassinPlot

What typical packages required to compile mocassin on linux:

    gcc openmpi

or

    intel/mpi

How to clean:

    make clean
     
How to run:

    mpirun -np N ./mocassinVoronoi

where N is number of processors for parallel computing.

How to run mpirun on a supercomputer:

In the [batches folder](https://github.com/equib/mocassin-models/tree/master/batches) of [mocassin-models](https://github.com/equib/mocassin-models), there are running batch examples for different job scheduling systems. 

To submit a batch file on the Portable Batch System (*PBS*):

     qsub mocassin_run.job

To submit a batch file on the Sun Grid Engine (*SGE*):

     qsub mocassin_run.job

To submit a batch file on the Simple Linux Utility for Resource Management (*SLURM*): 

     sbatch mocassin_run.sh

### References

* Hubber, D. A., Ercolano, B., & Dale, J., "Observing gas and dust in simulations of star formation with Monte Carlo radiation transport on Voronoi meshes", [MNRAS, 456, 756, 2016](http://adsabs.harvard.edu/abs/2016MNRAS.456..756H)
