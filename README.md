# optimization_routine
Optimization routine of material and friction coefficients of FE models of the Achilles tendon.

This routine was developed to optimize the material and friction parameters of Achilles tendon models based on in vivo displacement data. The Achilles tendon is represented as comprising three subtendons, corresponding to the three muscles of the triceps surae.

The routine begins by optimizing the material properties—specifically, three coefficients of the constitutive model—using displacement measurements of the free Achilles tendon acquired through ultrasound imaging. Following this, it optimizes the friction coefficients between the subtendons within the tendon model.

The routine can process multiple patients, taking their individual displacement data as input. The optimization process is implemented using Optuna [Akiba et al., 2019], and the script automatically saves the results of each run.

This workflow demonstrates how biomechanical parameters can be optimized within finite element (FE) models using subject-specific data. A detailed description of this work can be found in the published paper: https://www.sciencedirect.com/science/article/pii/S0021929025003367.
