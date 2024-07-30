---
title: "Project 1: N Body Simulation"
excerpt: "Efficient N-body Simulation Using Parallel Computing"
collection: portfolio
category: data-science
permalink: /portfolio/data-science-project-1

---

<div style="text-align: center;">
    <img src="/files/N_body_simulation_.gif" alt="nbody" width="400" />
</div>

## Overview

This project focuses on developing an efficient and accurate N-body simulation system using high-performance computing techniques. The N-body problem is crucial in fields like astrophysics, cosmology, and aerodynamics, involving the simulation of the motion of a system of particles under the influence of gravitational forces.

### Key Objectives

1. **Algorithm Development**: Create an N-body simulation algorithm that can be parallelized efficiently.
2. **Optimization**: Reduce communication overhead and load balancing issues in the parallelization process.
3. **High-Performance Implementation**: Implement the simulation on a high-performance computing architecture to handle large-scale systems.
4. **Scalability**: Investigate and ensure the scalability of the developed algorithm.

### Methodology

- **Cell Lists Algorithm**: Utilizes a grid of cells to reduce computational complexity by focusing on local interactions.
- **Leapfrog Time Integration**: Ensures accurate propagation of particle positions and velocities.
- **Parallelization Techniques**: Combines OpenMP for parallel processing within nodes and MPI for communication between nodes.
- **Performance Analysis**: Conducts roofline and scaling analyses to evaluate the efficiency and scalability of the algorithm.

### Findings

- **Efficiency Gains**: The parallelized algorithm demonstrates significant improvements in computation time.
- **Scalability**: The algorithm scales well with the number of processors, though efficiency decreases with increased communication overhead.

### Conclusion

The project successfully develops a highly scalable and efficient N-body simulation system, advancing the computational techniques available for simulating large-scale particle interactions.

### Repository and Resources

<!-- For more details and access to the code, please visit the [GitHub Repository](#). -->

To read the full analysis, you can download the [PDF file](/files/N_body_simulation.pdf).

---

<!-- ![Simulation Visualization 1](/files/N_body_simulation_.gif) -->

