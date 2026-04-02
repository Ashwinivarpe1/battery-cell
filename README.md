# Thermal Battery Simulation Project

This repository contains code and resources for simulating a thermal battery system. The project is structured as follows:

- `geometry/`: Contains definitions and generation scripts for the computational mesh.
- `solver/`: Implements the numerical solver for the thermal battery equations.
- `configs/`: Stores configuration files for parametric studies.
- `results/`: Output directory for simulation data (e.g., HDF5 files, VTU files).
- `visualization/`: Scripts for post-processing and visualizing simulation results.
- `notebooks/`: Jupyter notebooks for analysis and demonstrations.
- `docs/`: Project documentation.

## Getting Started

To set up the environment and run simulations, refer to the `environment.yml` file and the notebooks in the `notebooks/` directory.
The project began with the installation of Gmsh on Windows, where the first mesh file for the battery cell was successfully generated. This provided the geometric foundation for the simulations. From there, the work expanded into different environments: an attempt was made to run FEniCSx both on Linux and Google Colab, exploring its capabilities for numerical modeling. While these trials provided valuable insights, the focus then shifted to Elmer FEM, which offered a more suitable framework for conducting the thermal study of the battery cell.

With Elmer FEM, the thermal simulations were carried out, enabling a deeper understanding of heat distribution and management within the system. Building on this, the project progressed into a parameter study, where different conditions and variables were systematically tested to evaluate their impact on performance. This stage was crucial for identifying trends and optimizing the model.

Finally, the results were brought into ParaView, where visualization and validation took place. The graphical outputs allowed for clear interpretation of the simulations, and validation ensured that the computational results aligned with expectations and benchmarks. This sequence — from mesh generation, through solver exploration, thermal analysis, parameter studies, and visualization — established a complete workflow for battery cell modeling.

The project was then carefully organized into folders for configurations, geometry, solver inputs, results, and documentation. Once structured, it was uploaded to GitHub, making it version‑controlled, reproducible, and ready to share with collaborators. The repository now serves as a professional resource, containing all the essential components for others to explore, validate, and build upon.
