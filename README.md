# Computational Physics Project: Many Body Physics

**Author:** Ramit Goyal  
**Roll No:** 25B1049  
**Mentor:** Arnav Jain  
**Institution:** Maths and Physics Club, IIT Bombay  
**Date:** December 2025

## 📌 Project Overview

This repository contains simulations and analysis for critical phenomena in many-body physics systems. The project is divided into two core statistical mechanics modules: **Percolation Theory** (Geometric Phase Transitions) and the **Ising Model** (Thermodynamic Phase Transitions).

The simulations employ Monte Carlo methods, efficient cluster identification algorithms, and dimensionality reduction techniques to study phase transitions.

## 📂 Repository Structure

* **`CPP Part A.ipynb`**: Jupyter notebook for **Percolation Theory**. Includes lattice initialization, cluster labeling (Hoshen-Kopelman), and statistical analysis of percolation thresholds.
* **`CPP Part B.ipynb`**: Jupyter notebook for the **Ising Model**. Implements Single Spin Flip and Wolff cluster algorithms, optimized with Cython, and includes PCA analysis for phase separation.
* **`Report_Ramit_Goyal_CPP.pdf`**: Comprehensive project report detailing the theoretical background, derivations, algorithms, and results.

---

## 🔹 Part A: Percolation Theory

This module simulates **Site Percolation** on a 2D square lattice to analyze connectivity and geometric phase transitions.

### Key Features
* **Cluster Identification:** Implemented the **Hoshen-Kopelman algorithm** with Union-Find for efficient component labeling.
* **Phase Transition:** Analyzed the formation of spanning clusters to determine the critical occupation probability ($p_c$).
* **Statistical Metrics:** Calculated percolation strength ($P$), percolation probability ($\Pi$), and average cluster size ($S$).

**Result:** Estimated critical probability for site percolation: **$p_c \approx 0.59$**.

---

## 🔹 Part B: Ising Model

This module simulates the **2D Ising Model** to study ferromagnetism and thermodynamic phase transitions near the critical temperature ($T_c$).

### Key Features
* **Algorithms:** * **Metropolis-Hastings:** Single-spin flip dynamics.
  * **Wolff Algorithm:** Cluster-flip dynamics to mitigate critical slowing down.
* **Optimization:** computationally intensive loops optimized using **Cython**.
* **Analysis:**
  * Studied Magnetization ($M$), Susceptibility ($\chi$), and Specific Heat ($C_v$).
  * **PCA (Principal Component Analysis):** Applied to lattice configurations to visually separate ordered and disordered phases.

**Result:** Estimated critical temperature: **$T_c \approx 2.27$**.

---

## 🛠 Technologies Used

* **Python 3**
* **NumPy:** Vectorized lattice manipulations.
* **Matplotlib:** Visualization of phase transitions and lattice states.
* **SciPy:** Curve fitting and statistical analysis.
* **Scikit-learn:** Principal Component Analysis (PCA).
* **Cython:** Performance optimization for Monte Carlo steps.

## 🚀 How to Run

1. Download the jupyter files.
2. Install required dependencies:
   ``` bash
   pip install numpy matplotlib scipy scikit-learn cython jupyter
3. Launch Jupyter Notebook:
   ``` bash
   jupyter notebook
4. Open CPP Part A.ipynb or CPP Part B.ipynb to run the simulations.
   
