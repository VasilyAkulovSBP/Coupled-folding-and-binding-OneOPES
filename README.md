# Publication: Multimodal Conformational Landscape and Thermodynamics of Folding and Binding in an IDR

This repository contains the simulation input files, analysis scripts, and supporting materials associated with the following publication:

**Multimodal conformational landscape and thermodynamics of coupled folding and binding in an intrinsically disordered protein region**

**Authors:** Vasily Akulov, Valerio Rizzi, John van Noort, and Alireza Mashaghi.

## Citation

If you use any of the scripts, input files, or other materials provided in this repository, please cite the following publication:

https://doi.org/10.64898/2026.11.13.766518

## Repository Structure

The repository is organized into four main folders:

### 1. `Code/`

Contains Jupyter notebooks used to analyse the molecular dynamics (MD) simulation data and generate the figures presented in the publication.

### 2. `Folding/`

Contains the setup and input files for the OneOPES simulations of FCP1term in isolation (i.e., without RAP74).

Following the OneOPES framework, eight independent replicas were employed, with bias-sharing enabled between replicas. The PLUMED configuration files (`plumed_helix.dat`) can be found in the corresponding replica directories.

### 3. `Binding/`

Contains the setup and input files for the OneOPES simulations of the FCP1term–RAP74 complex.

In these simulations, FCP1term was subjected to structural restraints that maintained its helical conformation while allowing it to dissociate from RAP74 and explore the unbound state within the imposed restraints.

Following the OneOPES framework, eight independent replicas were employed, with bias-sharing enabled between replicas. The PLUMED configuration files (`plumed_helix.dat`) can be found in the corresponding replica directories.

### 4. `Folding_and_binding/`

Contains the setup and input files for the OneOPES simulations of the FCP1term–RAP74 complex, focusing on coupled folding and binding.

Unlike the simulations described in the `Binding/` folder, no structural restraints were applied to FCP1term, allowing it to freely explore different conformational states. Additionally, one extra supporting collective variable (CV) was included in the PLUMED configuration (`plumed_helix.dat`).

Following the OneOPES framework, eight independent replicas were employed, with bias-sharing enabled between replicas. The PLUMED configuration files (`plumed_helix.dat`) can be found in the corresponding replica directories.
