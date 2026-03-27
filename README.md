# Evolutionary MCMC for the Maximum Clique Problem (MCP)

## Overview

This repository provides an implementation of an **interaction-driven evolutionary Markov Chain Monte Carlo (MCMC)** framework for solving the **Maximum Clique Problem (MCP)**.

The method integrates:

* Evolutionary population-based search
* Gibbs / Metropolis probabilistic transitions
* Interaction-driven refinement mechanisms
* Efficient clique feasibility verification
* GPU-compatible design (optional)

The implementation is designed to run directly in **Google Colab** without requiring complex setup.

---

## Google Colab Usage

This project can be executed directly in **Google Colab**.

### Steps:

1. Open Google Colab.
2. Upload the file:

   ```
   keller_codes_d6.data
   ```
3. Upload the main source file (e.g., `.cpp` or `.cu`).
4. Compile and run inside a Colab cell.

### Example (C++)

```bash
g++ -O3 -std=c++17 main.cpp -o mcp
./mcp keller_codes_d6.data
```

If using CUDA (GPU runtime enabled in Colab):

```bash
nvcc -O3 main.cu -o mcp_gpu
./mcp_gpu keller_codes_d6.data
```

No additional folder structure is required.
Simply upload the data file and source code into the Colab session.

---

## Scientific Motivation

The **Maximum Clique Problem** is a classical NP-hard combinatorial optimization problem with applications in:

* Graph theory
* Coding theory
* Network analysis
* Computational geometry
* Combinatorial optimization

Dense structured graphs such as Keller graphs present significant computational challenges.
This project explores a probabilistic evolutionary alternative based on MCMC dynamics and interaction-driven refinement.

---

## Methodological Contributions

* Population-based evolutionary search
* Gibbs-style probabilistic updates
* Metropolis acceptance mechanism
* Energy-based clique evaluation
* Efficient adjacency and feasibility checks
* Optional GPU parallelization

---

## Reproducibility

* Supports fixed random seeds
* Deterministic mode (optional)
* Designed for lightweight experimental replication in Colab

---

## Authors

**Bouneb Zine El Abidine**
University of Oum El Bouaghi
Algeria
Email: [bouneb.zineabidine@univ-oeb.dz](mailto:bouneb.zineabidine@univ-oeb.dz)

**Talbi Hichem**
University of Constantine 2
Algeria

---

## Citation

If you use this repository in academic work, please cite:

```
Bouneb, Z. E. A., & Talbi, H.
Interaction-Driven Evolutionary MCMC for the Maximum Clique Problem.
Journal / Preprint, Year.
```

(Full citation details will be updated upon publication.)

---

## License

This project is released under the MIT License.

